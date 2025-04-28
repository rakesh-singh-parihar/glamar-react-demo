# GlamAR SDK React Integration

This repository provides a ready-to-use example for integrating the GlamAR Virtual Try-On (VTO) SDK into a React application.

GlamAR allows users to virtually try on eyewear, makeup, and accessories using augmented reality (AR) via a web browser.

---

## Quick Start

Follow the steps below to clone this repository, set up, and run the project locally:

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/glamar-react-integration.git
```

Then navigate into the project folder:

```bash
cd glamar-react-integration
```

### 2. Install dependencies

```bash
npm install
```

This command installs all required packages including React and related tooling.

### 3. Configure your GlamAR Access Key

Open the file `src/GlamARViewer.js` and locate the following line:

```javascript
window.GlamAR.init(
  containerRef.current.id,
  'YOUR_ACCESS_KEY', // <-- Replace this
  { ...options }
);
```

Replace `'YOUR_ACCESS_KEY'` with the actual access key provided by GlamAR.

### 4. Start the development server

Once the access key is updated, start your application:

```bash
npm start
```

The application will launch at:

```
http://localhost:3000
```

You will see the GlamAR Virtual Try-On application running.

---

## Project Structure

```
glamar-react-integration/
├── public/
│   └── index.html        # Loads GlamAR SDK script
├── src/
│   ├── GlamARViewer.js    # Main GlamAR SDK integration component
│   ├── App.js             # Root app component
│   ├── index.js           # React application entry point
│   └── index.css          # (optional) Basic styling
├── package.json           # Project metadata and scripts
└── README.md              # Project documentation
```

---

## Important Notes

- **Access Key**: The Access Key is mandatory to initialize the GlamAR SDK. Make sure it is kept secure.
- **SKU IDs**: Only valid SKU IDs configured in the GlamAR backend will load correctly.
- **Camera Permissions**: The browser must be allowed to access the user's camera for the AR experience to function.
- **Styling**: Feel free to modify the button layouts, container size, and styles in `GlamARViewer.js` according to your branding or project needs.

---

## References

- [GlamAR SDK Official Documentation](https://www.glamar.io/docs/VTO_web_integration_setup/)
- [React Documentation](https://react.dev/)

---

## Support

For access key generation, configuration support, or troubleshooting,  
please contact the GlamAR support team via [GlamAR Contact](https://www.glamar.io/contact).

---

## Summary

- Clone the repository
- Install dependencies
- Update your Access Key
- Start the development server
- Ready to use the GlamAR Virtual Try-On!

---

## Example Commands

```bash
git clone https://github.com/YOUR_USERNAME/glamar-react-integration.git
cd glamar-react-integration
npm install
# Update Access Key inside src/GlamARViewer.js
npm start
