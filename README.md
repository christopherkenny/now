
# now Publishers Article Quarto Template

Research article submission template. Template for nearly 20 journals, including the [Quarterly Journal of Political Science](https://www.nowpublishers.com/QJPS), the [Journal of Political Institutions and Political Economy](https://www.nowpublishers.com/PIP), and the [Journal of Historical Political Economy](https://www.nowpublishers.com/HPE).

## Creating a New Article

To create a new article using this format:

```bash
quarto use template christopherkenny/now
```

This will create a new directory with an example document that uses this format.

## Using with an Existing Document

To add this format to an existing document:

```bash
quarto add christopherkenny/now
```

Then, add the format to your document options:

```yaml
format:
  now-pdf: default
```    

## Options

*TODO*: If your format has options that can be set via document metadata, describe them.

## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

<!-- pdftools::pdf_convert('template.pdf',pages = 1) 
![[template.qmd](template.qmd)](template_1.png) -->

