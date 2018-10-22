# Deploying a React app with Surge

1. Make sure you have surge installed globally

- `npm install -g surge`

2. Run the Create React App build

- `cd your-react-project`
- `npm run build`

3. Change into build directory

- `cd build`

4. Run surge

- `surge`

### Adding deploy script to package.json

- In package.json under "scripts" add this line:
- `"deploy": "npm run build && surge ./build/ your-surge-url.surge.sh"`
- Update your-surge-url
- `npm run deploy` (this will need to be run from your project root, not the build directory)

## Technologies

- React built with Create-React-App
- CSS Animation adapted from [this pen by Mark Thomes](https://codepen.io/WithAnEs/pen/OVZRvg)
