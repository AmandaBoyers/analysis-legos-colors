# LEGO Datasets

This project analyzes LEGO datasets using various data processing and visualization techniques.

## Requirements

- Python 3.x
- matplotlib
- numpy
- pandas
- seaborn
- os
- zipfile
- display, Image from Ipython.display
- urlopen from urllib.request
- BytesIO from io import

# LEGO color exploration: How have LEGO piece colors changed since 1949?

## This notebook explores the following:

* The most common lego colors of all time (1950 to 2017)
* How the colors included in sets have changed over time
* How the size of sets have changed over time

## Other ideas for the LEGO data set

* Track popular themes and by year
* What colors are associated with which themes? 
* Could you predict which theme a set is from just by the bricks it contains?
* What sets have the most-used pieces in them? What sets have the rarest pieces in them?

## Data source

#### The data for this exploration comes from [Rebrickable](https://rebrickable.com/downloads/) which is a website that uses the lego datasets to show you which LEGO Sets you can build from the sets and parts you own.  The data is updated daily. The relational datasets available for download include themes, a color index, part_categories, parts, sets, minifigs, inventories, inventory_parts, inventory_sets, inventory_minifigs and a visual schema showing how the datasets connect to each other.  This exploration merges four datasets: the color index, inventories, inventory parts and sets.

## Data limitations

#### The data represents a catalog of what LEGO has produced in the past.  While we can get a sense of what was popular by what LEGO choose to create in any given year, we do not have sales data.  A sudden upward trend and then reduction the next year might suggest LEGO tried something new that didn't work, but without the sales data we only know what was created any given year.  For example, the data only tells us when a set was introduced, not how long it was in production or how successful it was in terms of sales.

## Usage

1. Clone the repository:
   ```sh
   git clone https://github.com/AmandaBoyers/Project.git

2. Navigate to the project directory:
    cd repository

3. Install the required packages:
        pip install -r requirements.txt

4. Run the Jupyter Notebook:

        jupyter notebook LEGO_Datasets.ipynb

License

This project is licensed under the MIT License.