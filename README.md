
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

This template supports standard author and affiliation schema.
For affiliations, please ensure that you use numeric IDs for codes, or they will print with extra text.

Standard fields, as listed below, are also supported:

- `title`: Title of your article
- `abstract`: Abstract of your article
- `keywords`: Keywords for your article
- `bibliography`: a path to your bibliography file, e.g. `references.bib`
- `acknowledgements`: Acknowledgements for your article

Note that acknowledgements *only* show if there is a corresponding author due to limitations of the underlying LaTeX template.

### Journal-specific options

Each of these should be placed under the `journal:` name.

For example,

```yaml
journal:
  name: "Journal of Example Studies"
```

- `code`: The unique code for your journal, e.g. `qjps` for the Quarterly Journal of Political Science.
- `issue-volume-year`: Year your journal issue was published
- `issue-volume-number`: Volume and issue numbers
- `disclaimer`: Optional legal/editorial disclaimer
- `data-box`: Submission dates, ISSN, and DOI information
- `copyright`: Copyright notice and publication year
- `title`: Official full title of your journal
- `shorttitle`: Short title or abbreviation of the journal
- `url`: Link to your journal homepage
- `issnprint`: Print edition ISSN identifier
- `issnonline`: Online edition ISSN identifier
- `aimsandscope`: Brief description of journal’s purpose and content
- `submission`: Instructions for journal submissions
- `abstractedin`: Databases/indexes that abstract your journal

## Example

Here is the source code for a minimal sample document: [template.qmd](template.qmd).

<!-- pdftools::pdf_convert('template.pdf',pages = 1) -->
![[template.qmd](template.qmd)](template_1.png)

## License

