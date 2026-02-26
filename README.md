# Pecha PDF Printer

A browser-based tool to reorder and impose PDF pages for Tibetan pecha printing. Works on **Mac, Windows, Linux** — any device with a modern browser. No installation required.

## Features

- **Upload any PDF** — drag & drop or click to browse
- **Automatic page padding** — adds blank pages to reach the required multiple (6 for pechas, 12 for mini pechas)
- **Pecha page reordering** — applies the correct print string so pages stack properly when printed double-sided
- **Imposition (n-up)** — places multiple pages per sheet, ready to print
- **100% client-side** — your files never leave your computer

## Format options

| Format | Layout | Pages per sheet | Multiple |
|--------|--------|-----------------|----------|
| A4 Landscape Pechas | 1×3 stacked | 3 | 6 |
| Mini Pecha | 2×3 grid | 6 | 12 |
| A4 Portrait Pecha | 1×6 stacked | 6 | 6 |
| Reorder Only | No imposition | 1 | 6 |

## Usage

1. Open `index.html` in your browser (or visit the GitHub Pages link)
2. Upload your pecha PDF
3. Choose a format
4. Click **Generate Pecha PDF**
5. Download the result and print

## How it works

The page reordering algorithm is based on the original FormatStringPrint.exe Windows tool used by the Longchen Nyingtik Project. For a 6-page pecha, for example, the print string is `1,3,5,6,4,2` — meaning:

- **Sheet 1 front** (top to bottom): pages 1, 3, 5
- **Sheet 1 back** (top to bottom): pages 6, 4, 2

This ensures that when printed double-sided and cut, the pages stack in the correct reading order.

## Credits

Longchen Nyingtik Project · [Lotsawa House](https://www.lotsawahouse.org)

Built with [pdf-lib](https://pdf-lib.js.org/).
