<template>
    <div>
        <h1>Data from Google Spreadsheet</h1>
        <table>
            <thead>
                <tr>
                    <th>Column 1</th>
                    <th>Column 2</th>
                    <th>Column 3</th>
                </tr>
            </thead>
            <tbody>
                <tr v-for="row in spreadsheetData" :key="row[0]">
                    <td>{{ row[0] }}</td>
                    <td>{{ row[1] }}</td>
                    <td>{{ row[2] }}</td>
                </tr>
            </tbody>
        </table>
    </div>
</template>

<script>
export default {
    data() {
        return {
            spreadsheetData: []
        };
    },
    async mounted() {
        await this.fetchDataFromSpreadsheet();
    },
    methods: {
        async fetchDataFromSpreadsheet() {
            try {
                const { google } = require('googleapis');

                // Load the credentials from a JSON file (replace 'credentials.json' with your own file)
                const auth = new google.auth.GoogleAuth({
                    keyFile: 'credentials.json',
                    scopes: ['https://docs.google.com/spreadsheets/d/1fmkVSp_yGS-7GsqsiXDTHYF714pKiMZQYuwosmUjGaE/edit?resourcekey#gid=1629831443']
                });

                // Create a client instance
                const client = await auth.getClient();

                // Create a Google Sheets API instance
                const sheets = google.sheets({ version: 'v4', auth: client });

                // Specify the spreadsheet ID and range of cells to retrieve
                const spreadsheetId = 'YOUR_SPREADSHEET_ID';
                const range = 'Sheet1!A1:C10';

                // Fetch the data from the spreadsheet
                const response = await sheets.spreadsheets.values.get({
                    spreadsheetId,
                    range
                });

                // Extract the values from the response
                const values = response.data.values;

                // Update the spreadsheetData array with the fetched data
                this.spreadsheetData = values || [];
            } catch (error) {
                console.error('Error fetching data:', error);
            }
        }
    }
};
</script>
