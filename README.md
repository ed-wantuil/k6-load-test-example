# k6 Load Test Example

This repository provides a practical example of load testing using [k6](https://k6.io/), a modern open-source performance testing tool for developers. It complements the article “[Is your system ready for peak load, or will it abandon users when they need it most?](https://medium.com/@ed-wantuil/is-your-system-ready-for-peak-load-or-will-it-abandon-users-when-they-need-it-most-c8b08f966189)” published on Medium.

## 📖 About

The goal of this project is to demonstrate how to structure and run realistic load tests that simulate user behavior during traffic spikes, helping you identify bottlenecks and ensure your system is scalable and resilient.

## 🚀 Technologies

- [k6](https://k6.io/)
    
- JavaScript (for writing test scripts)
    
- Docker (optional, for isolated local execution)
    

## 📂 Project Structure

``` bash
.
├── scripts/
│   ├── basic-test.js         # Basic test with a few users
│   ├── spike-test.js         # Spike test simulating a sudden traffic surge
│   ├── stress-test.js        # Stress test with gradually increasing load
│   └── ...
├── docker-compose.yml        # Docker environment for running k6
└── README.md                 # This file

```

## 🧪 How to Use

### Prerequisites

- k6 installed, **or**
    
- [Docker](https://www.docker.com/) installed
    

### Running a Test

#### Using k6 locally

``` bash
k6 run scripts/basic-test.js
```

### Customizing Tests

You can modify the scripts inside the `scripts/` directory to match your specific testing scenarios by adjusting parameters like `vus` (virtual users), `duration`, ramp-up stages, etc.

## 📈 Test Examples

- `basic-test.js`: A smoke test to validate the system is responding correctly.
    
- `spike-test.js`: Simulates a sudden spike in traffic.
    
- `stress-test.js`: Gradually increases load to identify the system’s breaking point.
    

## 📘 Related Article

For a deeper explanation of the **why** behind these tests and how to apply them effectively, check out the full article:

📄 [Is your system ready for peak load?](https://medium.com/@ed-wantuil/is-your-system-ready-for-peak-load-or-will-it-abandon-users-when-they-need-it-most-c8b08f966189)

## 🤝 Contributions

Contributions are welcome! Feel free to open issues, pull requests, or suggest improvements to the test scripts.

## 📄 License

This project is licensed under the MIT License.
