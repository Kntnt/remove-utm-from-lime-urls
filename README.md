# remove-utm-from-lime-urls

A Bash script that removes UTM tracking parameters from Lime Newsletter's special URLs.

## Usage

Before using the script for the first time, make it executable:

```bash
chmod +x remove-utm-from-lime-urls
```

This script requires exactly one parameter: the path to the file you want to process.

```bash
./remove-utm-from-lime-urls path/to/your/file.html
```

## Features

- Removes unwanted UTM parameters from special Lime Newsletter URLs
- Creates a ZIP file of the processed file for easy distribution

## Example

If your file contains URLs like:

```
$$share.public_url$$?utm_source=newsletter&utm_medium=email
```

The script will transform them to:

```
$$share.public_url$$
```
