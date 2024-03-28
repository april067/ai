# ai

https://github.com/taniarascia/webpack-boilerplate

# index.js

// Test import of a JavaScript module import { example } from '@/js/example';

// Test import of an asset import webpackLogo from '@/images/webpack-logo.svg';

// Test import of styles import '@/styles/index.scss';

// Appending to the DOM const logo = document.createElement('img'); logo.src =
webpackLogo;

const heading = document.createElement('h1'); heading.textContent = example();

// Test a background image url in CSS const imageBackground =
document.createElement('div'); imageBackground.classList.add('image');

// Test a public folder asset const imagePublic = document.createElement('img');
imagePublic.src = '/assets/example.png';

const app = document.querySelector('#root'); app.append(logo, heading,
imageBackground, imagePublic);

# /js/example.js

export const example = () =>
`Sensible webpack 5 boilerplate using Babel and PostCSS with a hot dev server    and an optimized production build.`;

# /styles/index.scss

@font-face { font-family: 'Inter'; src: url('../fonts/Inter.ttf'); }

@import 'variables'; @import 'scaffolding';

# /styles/variables.scss

$font-size: 1rem;
$font-family: 'Inter', sans-serif;
$background-color: #121212;
$font-color: #dae0e0; $page-width: 650px;

# /styles/scaffolding.scss

html { font-size:
$font-size; font-family: $font-family; background:
$background-color; color:
$font-color; line-height: 1.4; }

body { margin: auto; text-align: center; max-width: $page-width; }

h1 { margin: 0 0 2rem; }

.image { display: inline-block; height: 100px; width: 100px; background-image:
url('~assets/example.png'); background-size: cover; }
