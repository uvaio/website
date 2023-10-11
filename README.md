# UVA Information Organisation

> Web-based one-pager and visualisation for the Information Organisation course at the University of Amsterdam.

![GitHub banner](/docs/banner.jpg)

## Description

Informational webpage and visualiation to explore the dataset of the archaeological finds of the north / southline ([below the surface project](https://belowthesurface.amsterdam/en)) and organize the collection of content in new ways. Project structure built with [SvelteKit](https://kit.svelte.dev) and charts created with [Chart.js](https://www.chartjs.org). Any content from Below the Surface belong to the original copyright holders. Any data used is publically avaiable and can be downloaded from the original project website.

## Install

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/en) and NPM installed on your local machine.

### Running

```
# start a development server with hmr
npm run dev

# build a statis version of the site
npm run build
```

See `package.json` for further run scripts.A live version of the application is hosted on Netlify which uses the Svelte auto adapter for deployment.

## Project Structure

```
├── src                   # Svelte root folder
│   ├── components        # Svelte components
│   ├── datasets          # Raw .json files for data
├── static                # Fonts, images etc.
└── README.md

```

## License

Unless stated otherwise, code is [MIT][LICENSE] © [Danny de Vries](https://github.com/dandevri) & docs and images are [CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/).
