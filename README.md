# Bus Arrival Information

This is a simple, self-contained web application that displays upcoming bus arrivals for a given bus stop in Singapore. Users can enter a bus stop ID and the application will fetch and display arrival times from the ArrivaLah API. It also allows for filtering by specific bus service numbers.

## Demo

A live demo is available here: [https://yapweijun1996.github.io/SG-Bus-Arrival-Time-By-Bus-Code/](https://yapweijun1996.github.io/SG-Bus-Arrival-Time-By-Bus-Code/)

## Features

- **Default Bus Stop ID:** Automatically defaults to bus stop `70049` if no ID is provided in the URL.
- **Dynamic Search:** Enter a bus stop ID to get the latest arrival times.
- **Bus Service Filtering:** Filter the results by one or more bus service numbers using a simple tag-based input.
- **Auto-Refresh:** The arrival data automatically refreshes every 15 seconds.
- **Responsive Design:** The layout is optimized for both desktop and mobile devices.
- **User-friendly UI:** An intuitive interface with loading indicators and error messaging.
- **Detailed Information:** Displays bus service number, operator, estimated arrival times, load, bus type, and accessibility features.
- **URL-based State:** The bus stop ID and filters are stored in the URL, so you can share or bookmark your queries.

## Structure

This project is a single-file application.
- **`index.html`:** Contains all the necessary HTML, CSS, and JavaScript. There are no external stylesheets or script files.

## How It Works

1.  When the page loads, the application checks for a bus stop ID and any bus number filters from the URL query parameters. If no bus stop ID is found, it defaults to `70049`.
2.  It fetches bus arrival data from the ArrivaLah API using the specified bus stop ID.
3.  The data is processed and displayed on the page. If bus service filters are present, only the matching services are shown.
4.  The application then polls the API every 15 seconds to keep the arrival times up-to-date.
5.  Users can enter a new bus stop ID or add/remove bus service filters to get new results.

## Usage

1.  Clone the repository:
    ```bash
    git clone https://github.com/yapweijun1996/SG-Bus-Arrival-Time-By-Bus-Code.git
    ```
2.  Navigate to the project directory:
    ```bash
    cd SG-Bus-Arrival-Time-By-Bus-Code
    ```
3.  Open `index.html` in your web browser.

## Legend

The application uses the following abbreviations:

-   **Operator:**
    -   `SBST` – SBS Transit
    -   `SMRT` – SMRT Corporation
    -   `TTS` – Tower Transit Singapore
    -   `GAS` – Go Ahead Singapore
-   **Load:**
    -   `SEA` – Seats Available
    -   `SDA` – Standing Available
    -   `LSD` – Limited Standing
-   **Feature:**
    -   `WAB` – Wheelchair Accessible Bus
-   **Type:**
    -   `SD` – Single Deck
    -   `DD` – Double Deck
    -   `BD` – Bendy

## API

This application uses the ArrivaLah API:
`https://arrivelah2.busrouter.sg/?id={bus_stop_id}`

Replace `{bus_stop_id}` with the desired bus stop ID.

## License

This project is licensed under the MIT License.
