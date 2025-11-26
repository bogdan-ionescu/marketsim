# Market Simulator

A lightweight HTML + JavaScript market simulator that renders a live order book, candlestick price action, and cumulative depth curves. Orders are generated at random every 0.5 seconds within 3% of the latest trade price; takers cross the spread to consume resting liquidity while makers replenish the book.

## Usage

Open `index.html` in a browser. No build tooling is required because all dependencies load from CDNs. If your browser blocks CDN
scripts when opening from `file://`, start a tiny local server such as `python -m http.server 8000` in this directory and browse
to `http://localhost:8000/`.

* The **candlestick chart** renders locally (no extra plugin needed) and updates whenever trades occur.
* The **depth overlay** shows cumulative bid/ask liquidity from the simulated order book.
* **Order flow counters** reset each minute to highlight maker vs taker activity.
