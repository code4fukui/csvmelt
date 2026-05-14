# csvmelt

> 日本語のREADMEはこちらです: [README.ja.md](README.ja.md)

A browser-based tool to unpivot (or "melt") a wide CSV file into a long one. Convert horizontally-oriented data to a vertical, tidy format directly in your browser.

## Demo

[**Live demo**](https://code4fukui.github.io/csvmelt/)


![Screenshot of csvmelt UI](https://code4fukui.github.io/csvmelt/csvmelt.png)


## Features

-   **Interactive Unpivoting:** Convert wide data to long format. Select columns to keep as fixed identifiers, and the rest are "melted" into key-value pairs.
-   **Drag & Drop Interface:** Simply drop your CSV file to get started.
-   **Client-Side Processing:** All operations run locally in your browser. Your data is never uploaded to a server.
-   **Data Cleaning Options:**
    -   Trim leading/trailing whitespace from all cells.
    -   Sanitize numbers by removing thousands separators (commas).
    -   Remove empty rows and trailing empty columns.
-   **Encoding Support:** Automatically detects and handles common encodings like Shift_JIS and UTF-8.
-   **Custom Output:** Define custom names for the new variable and value columns.

## Usage

1.  Drag and drop a single CSV file onto the application page.
2.  (Optional) Check the desired data cleaning options (trim whitespace, remove commas, etc.) before dropping the file.
3.  Select columns to **discard** completely.
4.  Select columns to **keep** as fixed identifiers. All other columns will be unpivoted.
5.  Enter the new column names for the unpivoted "variable" and "value" data.
6.  Click "Convert". The resulting CSV file will be downloaded.

## Requirements

-   A modern web browser (e.g., Chrome, Firefox, Safari, Edge).
-   JavaScript must be enabled.

## Data / API

This project does not use any external data or APIs. All processing is done in the browser.

## License

MIT License — see [LICENSE](LICENSE).