
# Bus Arrival Information

This is a simple web application that displays upcoming bus arrivals for a given bus stop. Users can enter a bus stop ID and the application will fetch and display arrival times from the ArrivaLah API.

## Features

- **Default Bus Stop ID:** Automatically defaults to bus stop `70049` if no ID is provided.
- **Dynamic Search:** Enter a bus stop ID into the search bar to get updated arrival times.
- **Responsive Design:** Works across devices with a clean and modern layout.
- **User-friendly UI:** Intuitive interface with loading indicators and error messaging.
- **Data Display:** Shows bus service number, operator, estimated arrival times, and load/monitoring details.

## Structure

- **HTML (`index.html`):** Contains the structure of the web page, including a form for bus stop ID input and sections to display bus arrival services.
- **CSS (`styles.css`):** Provides styles for the layout, header, search form, bus service cards, and responsive design adjustments.
- **JavaScript (`script.js`):** Handles page interactivity, fetching data from the ArrivaLah API, and updating the DOM with bus arrival details.

## How It Works

1. When the page loads, the application checks for a bus stop ID in the URL query parameters. If none is found, it defaults to `70049`.
2. It then fetches bus arrival data from the ArrivaLah API using the bus stop ID.
3. The data is processed and displayed on the page, showing multiple bus services with their respective arrival times and details.
4. Users can enter a new bus stop ID and click "Check Arrival" to update the view accordingly.

## Usage

1. Clone the repository and navigate to the project directory:
   ```
   git clone https://github.com/yourusername/bus-arrival-information.git
   cd bus-arrival-information
   ```

2. Open `index.html` in your browser:
   - Either double-click the file or run a live server in your code editor.

3. Enter a bus stop ID in the input box to fetch and display the latest bus arrival information.

## API

This application uses the ArrivaLah API:
```
https://arrivelah2.busrouter.sg/?id={bus_stop_id}
```
Replace `{bus_stop_id}` with the desired bus stop ID.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

- The ArrivaLah API for providing bus arrival data.
- Google Fonts for the `Roboto` font.

## Demo
https://yapweijun1996.github.io/SG-Bus-Arrival-Time-By-Bus-Code/

