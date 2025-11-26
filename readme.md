# Market Simulator

A lightweight HTML + JavaScript market simulator that renders a live order book, candlestick price action, and cumulative depth curves. Orders are generated at random every 0.5 seconds within 1% of the latest trade price; takers cross the spread to consume resting liquidity while makers replenish the book.

## Usage

Open `index.html` in a browser. No build tooling is required because all dependencies load from CDNs.

* The **candlestick chart** uses the Chart.js financial plugin and updates whenever trades occur.
* The **depth overlay** shows cumulative bid/ask liquidity from the simulated order book.
* **Order flow counters** reset each minute to highlight maker vs taker activity.
