# EPL 2019-20 Player Performance Analysis

Exploratory data analysis of English Premier League 2019-20 season player
statistics, focused on forwards and midfielders. Filters and derives
performance metrics from raw stats, then visualizes the standout performers
of the season.

## What's analyzed

**Forwards**
- Shot accuracy (shots vs. shots on target)
- Top scorers by total goals
- Goals per match (players with the highest scoring rate, not just volume)
- Most headed goals

**Midfielders**
- Assist leaders ("Assists Kings") among high-appearance, high-assist players
- Goal contributions from midfield

Each section filters players by a minimum appearance threshold before ranking,
so the results reflect regular starters rather than small-sample outliers.

## Visualizations

Built with Matplotlib and Seaborn: horizontal bar charts for top-10 rankings
(top scorers, headed goals, assists, goals-per-match), plus a subplot
comparison view combining multiple rankings side by side.

## Tech Stack

- **Python**
- **pandas** / **NumPy** — data wrangling and filtering
- **Matplotlib** / **Seaborn** — visualization
- **Jupyter Notebook**

## Running it

1. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```
2. The notebook expects a `pl_19-20.csv` file (2019-20 EPL player statistics)
   in a local `Datasets` folder — update the path in the second cell
   (`os.chdir(...)`) to point at your own copy of the dataset.
3. Open `Project EPL.ipynb` in Jupyter and run all cells.

## Project Structure

```
.
└── Project EPL.ipynb   # Full analysis: data prep, filtering, metrics, visualizations
```
