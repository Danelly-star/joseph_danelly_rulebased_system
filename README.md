# A2---Implement-a-Rule-Based-System - Danelly Joseph (301544396)
Github Repository Link:

# Generative Mosaic Pattern Designer

## Description

The Generative Mosaic Pattern Designer is an L-System-based generative art
project created for IAT 460. The program uses recursive production rules and
Turtle graphics to generate geometric motifs inspired by decorative mosaic
patterns.

The system currently includes four pattern families:

- Square Mosaic
- Star Mosaic
- Cross Mosaic
- Snowflake Mosaic

Each generated motif is repeated three times to create a tile-like pattern.

## Requirements

- Python 3
- Google Colab or Jupyter Notebook
- ColabTurtle

## How to Run

1. Open the `.ipynb` notebook in Google Colab.
2. Run the ColabTurtle installation cell.
3. Run the import cell.
4. Run the remaining function and pattern-definition cells in order.
5. Run one of the sample output cells to generate a mosaic.

The main function for generating a row of mosaic tiles is:

    generate_tile_row()

Example:

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
Controls the number of times the L-System production rules are applied.

`angle`
Controls the Turtle's turning angle.

`distance`
Controls the length of each drawn line segment.

`color`
Controls the color used when random color mode is disabled.

`thickness`
Controls line thickness.

`background`
Controls the canvas background color.

`random_colors`
Controls optional color randomization.

- `False` = all three motifs use the selected color.
- `True` = three different colors are randomly selected from the palette.

## Notes

Higher iteration values can cause some L-System patterns to become extremely
large because the instruction strings grow recursively. The provided sample
settings were selected to keep the patterns readable within the canvas.
