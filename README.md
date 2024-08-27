# Nokia One-Step Form

## Overview

This project is a single-page Vue.js application featuring a stylish form interface with Nokia branding. It's designed to collect user information in a sleek, responsive layout.

## Features

- Responsive design that works on both desktop and mobile devices
- Custom Nokia-themed styling with background image
- Form for collecting user's name, country, and provider
- "Remember Me" checkbox functionality
- Submission redirects to a specified URL
- This is done for the collecting username and selecting the country and provider to access.


## Prerequisites

Before you begin, ensure you have met the following requirements:

- Node.js (v12.0 or higher recommended)
- npm (usually comes with Node.js)

## Installation

To install this project, follow these steps:

1. Clone the repository:

```
git clone https://github.com/Cobalt9000/nokia-page-1-redirect.git
```

2. Navigate to the project directory:

```
cd nokia-page-1-redirect
```

3. Install the dependencies:

```
npm install
```
or you can also use ```npm i``` for installing dependencies.


## Usage

To run this project locally:

1. Start the development server:

```
npm run dev
```

2. Open your browser and visit `http://localhost:5173` (or the port shown in your terminal).

## Building for Production

To build the project for production:

```
npm run build
```

This will generate a `dist` folder with all the files ready for deployment.

## Customization

- To change the background image, replace `public/nokia.png` with your desired image.
- Modify the form fields in the `<template>` section of `App.vue` to collect different information.
- Adjust the styling in the `<style>` section of `App.vue` to match your branding requirements.

## Contributing

Contributions to this project are welcome. Please follow these steps:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature-name`)
3. Make your changes
4. Commit your changes (`git commit -am 'Add some feature'`)
5. Push to the branch (`git push origin feature/your-feature-name`)
6. Create a new Pull Request

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

If you have any questions or feedback, please open an issue in this repository.