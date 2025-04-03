# Wardriving Mapping Tool

A lightweight, browser-based application for mapping and managing vulnerable devices discovered during wardriving activities. This tool allows security researchers to document, visualize, and share information about potentially vulnerable devices on a map interface.

![Wardriving Mapping Tool Screenshot](screenshots/preview.png)

## 🚀 Features

- **Interactive Map**: Visualize device locations on an OpenStreetMap interface
- **Device Management**: Add, edit, and delete device entries with custom information
- **Location Tools**: Capture coordinates by clicking on the map or using your current location
- **Data Persistence**: All data is stored in the browser's localStorage
- **Import/Export**: Share your findings by exporting to JSON or import data from other sources
- **Responsive Interface**: Works on desktop and mobile devices
- **Offline Capable**: Once loaded, can be used without an internet connection (except for map tiles)
- **Privacy Focused**: All data stays on your device - no server communication required

## 📋 Device Information Tracking

For each vulnerable device, you can record:
- Name/identifier
- Device type (e.g., EM4100, WiFi AP, IP Camera)
- Detailed information (default passwords, vulnerabilities, etc.)
- Precise geolocation coordinates

## 🔧 Installation

This is a client-side web application with no server dependencies. To use it:

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/wardriving-mapping-tool.git
   ```

2. Open `index.html` in any modern web browser
   - For full functionality including geolocation, use a secure context (HTTPS or localhost)

### Optional Local Server Setup

For testing with full features, you may want to run a local server:

```bash
# Using Python
python -m http.server

# Using Node.js with http-server
npx http-server
```

## 📖 Usage Guide

### Adding Devices

1. Find the location on the map and click to set coordinates, or use "Use Current Location"
2. Fill in the device information in the sidebar form
3. Click "Add Device" to save the entry

### Managing Devices

- Click on any device in the sidebar list to center the map on that location
- Click on a map marker to view device details and access Edit/Delete options
- Use the Import/Export buttons to backup or share your dataset

### Data Management

- All data is stored in your browser's localStorage
- Use the Export button to save your data as a JSON file
- Use the Import button to load previously exported data or data from colleagues

## 🛠️ Technologies Used

- HTML5, CSS3, and JavaScript (ES6+)
- [Leaflet.js](https://leafletjs.com/) for interactive mapping
- [OpenStreetMap](https://www.openstreetmap.org/) for map tiles
- Browser APIs: Geolocation, LocalStorage, File API

## 🔒 Privacy & Ethical Use

This tool is intended for legitimate security research, penetration testing, and educational purposes. Always:

- Obtain proper authorization before scanning networks
- Follow local laws and regulations regarding wardriving and security testing
- Handle discovered vulnerabilities responsibly, following ethical disclosure practices
- Respect privacy and do not share sensitive information publicly

## 🤝 Contributing

Contributions are welcome! Feel free to submit issues or pull requests.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

**Disclaimer**: This tool is provided for educational and legitimate security research purposes only. Users are responsible for ensuring their use of this tool complies with all applicable laws and regulations.
