# Ignite UI Layout Manager arbitrary sizing PoC

This is a PoC of an arbitrary sizing in Ignite UI Layout Manager when using a grid layout.

## Implementation

Introduced two new properties to the `gridLayout` object: `columnsWidth` and `columnsHeight` which holds arrays of sizes for each column/row. You can set the sizes in px, percent or using asterisk (for filling the remaining space).

## Starting the sample

In order to start the sample get the repo and open __sample.html__.

## PoC Limitations

1. You should have `rows` and `cols` properties declared.
2. Only one `*` per `columnsWidth`/`columnsHeight` could be used.
3. Resizing the window is not supported.

## Tile Manager

Since the Tile Manager sits on top of the Layout Manger's grid layout, when the arbitrary sizing feature is implemented in the Layout Manager, it should be working in the Tile Manager out of the box.
