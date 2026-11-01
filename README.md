# Urban Economics Lab (ECON 348)

Interactive course notes for ECON 348: Urban Economics, written in Markdown (`.qmd` files) and built with [Quarto](https://quarto.org). Each topic page explains a model, has a simulation with sliders that runs in the browser (Observable JS, built into Quarto), and adds "Things to try," evidence from the assigned readings, a Maine example, an optional Network lens, and practice questions.

## Preview and build

Quarto 1.10.20 is installed at `~/opt/quarto-1.10.20/bin/quarto`. From this folder:

```bash
~/opt/quarto-1.10.20/bin/quarto preview
```

opens a live preview that refreshes as you edit. To build the finished site into `docs/`:

```bash
~/opt/quarto-1.10.20/bin/quarto render
```

## Publish

The site is hosted on GitHub Pages at <https://hitanshupandit.github.io/eco348-book/>, served from the `docs/` folder on the `main` branch. To update it after editing a page:

```bash
~/opt/quarto-1.10.20/bin/quarto render
git add -A
git commit -m "Update notes"
git push
```

GitHub Pages republishes automatically a minute or two after the push.

## Files

- `_quarto.yml`: site settings and the sidebar order
- `index.qmd`: overview page
- One `.qmd` per topic, in syllabus order: `why-cities`, `monocentric-city`, `extending-model`, `sprawl`, `congestion`, `tenure-choice`, `housing-supply`, `housing-policy`, `neighborhoods`, `pollution-crime`, `quality-of-life`, `place-based`
- `references.bib`: citations, all checked against their DOIs
- `styles.css`: garnet accents, simulation panels, and Network lens boxes
- `images/`: static figures
