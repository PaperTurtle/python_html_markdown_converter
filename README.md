# Markdown to HTML Converter

This tool is a versatile Python script for converting Markdown files to HTML and vice versa. It supports various features like custom titles, CSS styling, batch conversion, interactive mode, Markdown extensions, and HTML template customization.

## Features

-  Convert Markdown to HTML: Converts Markdown files to HTML format.
-  Convert HTML to Markdown: Converts HTML files back to Markdown format.
-  Custom Title for HTML: Allows specifying a custom title for the HTML document.
-  Custom CSS Styling: Link a custom CSS stylesheet for the HTML output.
-  Batch Conversion: Convert multiple files at once.
-  Interactive Mode: Run the tool in an interactive CLI mode for ease of use.
-  Markdown Extensions: Support for various markdown2 extensions.
-  HTML Template Customization: Use a custom HTML template for the output.

## Installation

1. Make sure to have Python installed on your machine
2. Clone or download this repository
3. Install the required packages

## Usage

The script can be used in the command line with various arguments to control its behavior.

### Basic Usage

-  Convert a single Markdown file to HTML:

```{python}
python converter.py input.md output.html --to_html
```

-  Convert a single HTML file to Markdown:

```{python}
python converter.py input.html output.md --to_md
```

### Advanced Usage

-  Batch Convert Markdown Files:

```{python}
python converter.py "\*.md" output_directory/ --to_html
```

-  Using a Custom Title and CSS File:

```{python}
python converter.py input.md output.html --to_html --title "My Custom Title" --css "style.css"
```

-  Enable Markdown Extensions:

```{python}
python converter.py input.md output.html --to_html --extensions "tables,footnotes"
```

-  Using an HTML Template File:

```{python}
python converter.py input.md output.html --to_html --template "template.html"
```

-  Interactive Mode:

```{python}
python converter.py --interactive
```

### Interactive Mode

When run in interactive mode, the script will prompt for inputs and options, making it easier for users who prefer not to use command line arguments.
