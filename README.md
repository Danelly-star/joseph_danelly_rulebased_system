# A2---Implement-a-Rule-Based-System - Danelly Joseph (301544396)
Github Repository Link:https://github.com/Danelly-star/joseph_danelly_rulebased_system.git

# Mosaic Pattern Tile Designer Using L-Systems

## Description

The Mosaic Pattern Tile Designer is L-System-based. The program uses recursive production rules and
Turtle graphics to generate geometric motifs inspired by decorative mosaic tile
patterns.

In the system I currently included four pattern options:

- Square Mosaic
- Star Mosaic
- Cross Mosaic
- Snowflake Mosaic

Each generated motif is repeated three times to create a tile-like adjacent pattern.

## Requirements

- Python 3
- Google Colab or Jupyter Notebook
- ColabTurtle

## How to Run

1. Open the notebook in Google Colab.
2. Run the ColabTurtle installation cells.
3. Run the import cell.
4. Run the remaining function and pattern-definition cells in order.
5. You can skip the test cells, unless if you want to see if it works. 
6. Run one of the sample output cells to generate a mosaic.

(Simply put, just run everything from top to bottom in order, as I have organized it that way)



## About the Functions

The main function for generating a row of mosaic tiles in the sample output is:

    generate_tile_row()

Example Structure:(If you want to make your own tile design, add a new empty cell at the bottom of the notebook and past the generate_tile_row() structure as shown below into your cell

    generate_tile_row(
        "cross",
        iterations=3,
        distance=5,
        color="teal",
        thickness=5,
        random_colors=False
    )

## Available Patterns

The following pattern names can be passed to `generate_tile_row()`:

- `"square"`
- `"star"`
- `"cross"`
- `"snowflake"`

## Adjustable Parameters

`iterations`
Controls the number of times the L-System production rules are applied. Cannot do no more than 3 iterations

`angle`
Controls the Turtle's turning angle.

`distance`
Controls the length of each drawn line segment. Distance cannot be more than 8 because the system will freeze

`color`
Controls the color used when random color mode is disabled or False.

`thickness`
Controls line thickness.

`random_colors`
Controls optional color randomization.

- `False` = all three motifs use the selected color in the color parameter.
- `True` = three different colors are randomly selected from the palette of colors I put. 

