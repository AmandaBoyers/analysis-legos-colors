# LEGO Datasets

# LEGO color exploration: How have LEGO piece colors changed since 1949?

This project analyzes how LEGO colors have changed over time using various data processing and visualization techniques.

![LEGOs Then and Now](images/ThenNow.png)


## Table of Contents
- [Requirements](#requirements)
- [LEGO color exploration: How have LEGO piece colors changed since 1949?](#lego-color-exploration-how-have-lego-piece-colors-changed-since-1949)
- [This notebook explores the following](#this-notebook-explores-the-following)
- [Other ideas for the LEGO data set](#other-ideas-for-the-lego-data-set)
- [Data source](#data-source)
- [Data loading and preprocessing](#data-loading-and-preprocessing)
- [Data limitations](#data-limitations)

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

## Data loading and preprocessing

#### The datasets were loaded using Pandas. The sets.csv contains set_num, name of the set, year, theme_id and the number of parts. Each set contains inventories, which consist of parts. (So, an inventory is like a bag of parts.) Each set can contain many inventories and each of those inventories can contain many parts. The data set inventory_parts has details on parts such as the part_num, color_id and quantity. The colors dataset is a color index that contains over 200 different colors. By merging sets, inventories, inventory_parts and colors we get a list of all parts, their colors, what sets they are part of, image urls for sets and parts and the year for each set.¶

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

<p align="center">
    <img src="images/RetroRollerSkateSet.png" alt="LEGOs Then and Now" width="50%">
</p>