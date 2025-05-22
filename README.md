# Smart Location IAQ Dashboard 🌿

Dashboard for monitoring Indoor Air Quality (IAQ) across multiple smart locations.

## 🚀 Live Demo

Once GitHub Pages is enabled, your dashboard will be available at:
**https://jigarthummar.github.io/Smart-Location-IAQ-Dashboard/**

## 📊 Features

- **Real-time Monitoring**: Live data visualization for CO₂, Temperature, Humidity, and TVOC levels
- **Interactive Charts**: Individual trend charts for each sensor with Chart.js
- **Status Indicators**: Color-coded status indicators based on air quality standards
- **Responsive Design**: Works on desktop, tablet, and mobile devices
- **Modern UI**: Glassmorphism design with smooth animations

## 🌡️ Monitored Parameters

- **CO₂ Level**: Carbon dioxide concentration (ppm)
  - Excellent: < 400 ppm
  - Good: 400-800 ppm
  - Fair: 800-1200 ppm
  - Poor: > 1200 ppm

- **Temperature**: Ambient temperature (°C)
  - Optimal: 20-24°C
  - Comfortable: 18-26°C
  - Suboptimal: Outside range

- **Humidity**: Relative humidity (%)
  - Ideal: 40-60%
  - Acceptable: 30-70%
  - Suboptimal: Outside range

- **TVOC**: Total Volatile Organic Compounds (ppb)
  - Excellent: < 220 ppb
  - Good: 220-660 ppb
  - Fair: 660-2200 ppb
  - Poor: > 2200 ppb

## 🛠️ Deployment Instructions

### Option 1: GitHub Pages (Recommended)

1. Go to your repository: https://github.com/jigarthummar/Smart-Location-IAQ-Dashboard
2. Click on **Settings** tab
3. Scroll down to **Pages** section in the left sidebar
4. Under **Source**, select **Deploy from a branch**
5. Choose **main** branch and **/ (root)** folder
6. Click **Save**
7. Wait a few minutes for deployment
8. Your dashboard will be available at: https://jigarthummar.github.io/Smart-Location-IAQ-Dashboard/

### Option 2: Local Development

1. Clone the repository:
   ```bash
   git clone https://github.com/jigarthummar/Smart-Location-IAQ-Dashboard.git
   cd Smart-Location-IAQ-Dashboard
   ```

2. Open `index.html` in your web browser or serve it with a local server:
   ```bash
   # Using Python
   python -m http.server 8000
   
   # Using Node.js
   npx serve .
   ```

3. Navigate to `http://localhost:8000` in your browser

## 🔧 Customization

### Connecting Real Data Sources

Currently, the dashboard uses simulated data. To connect real sensors:

1. Replace the `fetchSensorData()` function in `index.html`
2. Update the function to call your actual API endpoint
3. Ensure your API returns data in this format:
   ```javascript
   {
     "CO2": 450,
     "Temperature": 22.5,
     "Humidity": 55.0,
     "TVOC": 300,
     "Timestamp": 1640995200000
   }
   ```

### Styling Customization

- Modify CSS variables in the `<style>` section
- Change colors by updating the color codes in the metric cards
- Adjust chart colors in the `chartConfigs` object

## 📱 Browser Compatibility

- Chrome/Edge (recommended)
- Firefox
- Safari
- Mobile browsers

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 📞 Contact

Jigar Thummar - [LinkedIn](https://www.linkedin.com/in/jigar-thummar-aa22201b0)

Project Link: [https://github.com/jigarthummar/Smart-Location-IAQ-Dashboard](https://github.com/jigarthummar/Smart-Location-IAQ-Dashboard)
