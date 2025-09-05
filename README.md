# 📱 Sesi13 Anandayudhistira - Mobile App Testing Suite

[![Node.js](https://img.shields.io/badge/Node.js-18+-green.svg)](https://nodejs.org/)
[![WebdriverIO](https://img.shields.io/badge/WebdriverIO-9+-blue.svg)](https://webdriver.io/)
[![Appium](https://img.shields.io/badge/Appium-1.22+-purple.svg)](https://appium.io/)
[![Allure](https://img.shields.io/badge/Allure-Reporting-orange.svg)](https://docs.qameta.io/allure/)
[![License](https://img.shields.io/badge/License-ISC-yellow.svg)](./LICENSE)

## 📋 Overview

This project is an automated testing suite built with WebdriverIO and Appium for mobile application testing. It focuses on Android app testing using the Android API Demos application as a test subject, providing a robust framework for UI automation and regression testing.

## 🎯 Project Description

**Sesi13 Anandayudhistira** is a comprehensive mobile testing framework that:

- ✅ Automates Android app testing using WebdriverIO
- 📊 Generates detailed test reports with Allure
- 📸 Captures screenshots on test failures
- 🔧 Uses Mocha BDD framework for test organization
- 🚀 Supports local Appium server execution
- 📱 Tests on Android emulator (API level 16+)

The current test suite includes basic app launch verification, with extensible structure for adding more complex test scenarios.

## 🛠️ Installation

### Prerequisites

- **Node.js** (v18 or higher) - [Download here](https://nodejs.org/)
- **Appium Server** (v1.22+) - Install via npm: `npm install -g appium`
- **Android SDK** with emulator - [Android Studio](https://developer.android.com/studio)
- **Java JDK** (v8 or higher)

### Setup Steps

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd sesi13_anandayudhistira
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Start Appium Server:**
   ```bash
   appium --address 127.0.0.1 --port 4723
   ```

4. **Configure Android Emulator:**
   - Create an Android Virtual Device (AVD) with API level 16+
   - Start the emulator before running tests

## 🚀 Usage

### Running Tests

Execute the test suite using npm:

```bash
npm test
```

This will:
- Launch the Android emulator
- Install and start the API Demos app
- Run all test cases in the `tests/` directory
- Generate Allure test reports

### Test Structure

```
tests/
└── appdemo.test.js    # Basic app launch test
```

### Generating Reports

After test execution, generate and view Allure reports:

```bash
# Install Allure CLI (if not already installed)
npm install -g allure-commandline

# Generate report
allure generate allure-results --clean

# Open report in browser
allure open
```

## 💻 System Output Language

This project is developed using **JavaScript** with Node.js runtime environment. Key technologies include:

- **JavaScript (ES6+)** - Primary programming language
- **Node.js** - Runtime environment
- **WebdriverIO** - Test automation framework
- **Appium** - Mobile automation server
- **Mocha** - Test framework
- **Chai** - Assertion library

## 📊 Test Results

Test execution generates:
- Console output with real-time test progress
- Allure HTML reports with detailed test steps
- Screenshots captured on test failures (stored in `allure-results/`)

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the ISC License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For questions or issues, please open an issue in the repository or contact the development team.

---

*Built with ❤️ using WebdriverIO and Appium*
