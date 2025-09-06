# Squeal

Query CSV files with SQL directly in your browser - no server required.

## Features

- **Drag & Drop**: Upload CSV files by dragging or clicking
- **Smart Parsing**: Auto-detects delimiters (comma, semicolon, tab, pipe)
- **Flexible Headers**: Toggle whether first row contains headers
- **SQL Queries**: Full SQLite syntax support in your browser
- **Schema Inspector**: View column details and sample data
- **Privacy First**: All processing happens locally - your data never leaves your browser

## Usage

1. **Start the server**:
   ```bash
   python3 -m http.server 8000
   ```

2. **Open browser**: Navigate to `http://localhost:8000`

3. **Upload CSV**: Drag and drop or click to upload your CSV file

4. **Query data**: Use the SQL editor to query your data
   ```sql
   SELECT * FROM data WHERE age > 25
   SELECT department, COUNT(*) FROM data GROUP BY department
   ```

## Supported File Formats

- **CSV**: Comma-separated values
- **TSV**: Tab-separated values  
- **SSV**: Semicolon-separated values
- **PSV**: Pipe-separated values

## Quick Start Example

Try with this sample CSV:
```csv
name,age,city
Alice,30,New York
Bob,25,London
Carol,35,Tokyo
```

## Technology

- **SQLite WASM**: Full SQL database in the browser
- **TailwindCSS**: Modern, responsive UI
- **Vanilla JavaScript**: No framework dependencies
- **Local Processing**: Everything runs client-side

## License

MIT License - feel free to use and modify as needed.