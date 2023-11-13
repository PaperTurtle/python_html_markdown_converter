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

1. Ensure Python is Installed:
   Ensure that you have Python installed on your machine. This script is compatible with Python 3.
2. Clone or download this repository
   Clone or download this repository to your local machine.

   ```bash
   git clone https://your-repository-url
   cd path-to-your-repository
   ```

3. Install the required packages

   ```python
   pip install -r requirements.txt
   ```

## Usage

The script can be used in the command line with various arguments to control its behavior.

### Basic Usage

-  Convert a single Markdown file to HTML:

```python
python converter.py input.md output.html --to_html
```

-  Convert a single HTML file to Markdown:

```python
python converter.py input.html output.md --to_md
```

### Advanced Usage

-  Batch Convert Markdown Files:

```python
python converter.py "\*.md" output_directory/ --to_html
```

-  Using a Custom Title and CSS File:

```python
python converter.py input.md output.html --to_html --title "My Custom Title" --css "style.css"
```

-  Enable Markdown Extensions:

```python
python converter.py input.md output.html --to_html --extensions "tables,footnotes"
```

-  Using an HTML Template File:

```python
python converter.py input.md output.html --to_html --template "template.html"
```

-  Interactive Mode:

```python
python converter.py --interactive
```

### Interactive Mode

When run in interactive mode, the script will prompt for inputs and options, making it easier for users who prefer not to use command line arguments.

## Examples

1. Converting with Custom Title:

   -  Command: `python converter.py example.md example.html --to_html --title "Example Document"`
   -  This will convert example.md to example.html with the title "Example Document".

2. Batch Conversion:

   -  Command: `python converter.py "\*.md" converted_html/ --to_html`
   -  This will convert all .md files in the current directory to .html files and save them in the converted_html directory.

3. Using Custom CSS:
   -  Command: `python converter.py example.md example.html --to_html --css "mystyles.css"`
   -  Converts example.md to example.html applying styles from mystyles.css.

## Notes

-  When using a custom HTML template, ensure it contains {{content}} where you want the Markdown content to be injected.
-  The batch conversion feature assumes the output path is a directory.

## Contributing

Contributions to this project are welcome. Feel free to fork the repository and submit pull requests.

## Licence

[MIT](https://choosealicense.com/licenses/mit/)
