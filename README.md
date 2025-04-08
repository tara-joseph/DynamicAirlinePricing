# Dynamic Programming for Airline Ticket Sales

This project applies **dynamic programming** to optimize airline ticket sales and overbooking strategies, balancing revenue maximization with customer satisfaction. Airlines routinely face a trade-off: selling too few tickets risks empty seats, while overbooking can lead to costly passenger compensation and negative customer experiences. Our goal was to develop an intelligent pricing and booking policy that adapts over time and considers customer behavior, seat capacity, and financial risk.

## Key Features

- **Modeled Ticket Sales Probabilities** based on dynamic pricing, cabin class (coach vs. first-class), and remaining seat availability.
- **Incorporated Overbooking Costs** using real-world constraints (e.g., no-show probabilities, upgrade and bump-off penalties).
- **Simulated Multiple Strategies**:
  - Hard cap overbooking limits
  - Optional “no-sale” pricing days
  - Seasonal demand adjustments
  - A combined policy integrating all features
- **Optimized Profit** through backward induction, starting from the day of departure to determine the best sale decision for each preceding day.

## Results

- Identified the optimal overbooking cap (10 extra coach seats) across different policies.
- Achieved a maximum expected discounted profit of **$42,140.53** under the flexible "no-sale" strategy.
- Visualized trade-offs between overbooking frequency, kick-off rates, cost, and profit volatility.

## Tools & Technologies

- Python, NumPy, SciPy
- Dynamic Programming algorithms
- Simulation and data visualization for scenario comparisons
