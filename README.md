# PWM Rectifier Working Analysis in MATLAB

A comprehensive MATLAB simulation tool for analyzing three-phase PWM rectifier behavior, including duty cycle calculations, input phase current waveforms, and output power characteristics with detailed visualization of electrical parameters.

## 📋 Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Parameters](#parameters)
- [Results](#results)
- [Project Structure](#project-structure)
- [Performance Metrics](#performance-metrics)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [Authors](#authors)
- [License](#license)

## 🔍 Overview

This project implements a MATLAB-based simulation of a three-phase PWM rectifier system. The simulation analyzes the rectifier's behavior by calculating PWM signals, input phase currents, and output power characteristics. The tool provides comprehensive visualization of electrical parameters and performance metrics essential for power electronics analysis.

## ✨ Features

- **Three-phase PWM signal generation** with configurable switching frequency
- **Input phase current calculation** with sinusoidal waveform analysis
- **Output power computation** based on voltage and current interactions
- **Real-time parameter visualization** with multiple subplot displays
- **Performance metrics calculation** including RMS values and power statistics
- **Configurable system parameters** for different operating conditions
- **Comprehensive plotting** of PWM signals, currents, and power waveforms

## 🔧 Requirements

- MATLAB R2018b or later
- Signal Processing Toolbox (recommended)
- Control System Toolbox (optional)

## 📦 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/pwm-rectifier-analysis.git
   cd pwm-rectifier-analysis
   ```

2. Open MATLAB and navigate to the project directory

3. Run the main simulation file:
   ```matlab
   run('pwm_rectifier_analysis.m')
   ```

## 🚀 Usage

### Basic Usage

```matlab
% Simply run the main script
pwm_rectifier_analysis
```

### Custom Parameters

You can modify the following parameters in the script:

```matlab
fsw = 1e3;          % Switching frequency (Hz)
Vdc = 400;          % DC link voltage (V)
Vin_rms = 230;      % Input phase voltage (rms) (V)
Rload = 10;         % Load resistance (Ohm)
Lfilter = 1e-3;     % Filter inductance (H)
Cfilter = 100e-6;   % Filter capacitance (F)
```

## 📊 Parameters

| Parameter | Symbol | Default Value | Unit | Description |
|-----------|--------|---------------|------|-------------|
| Switching Frequency | `fsw` | 1000 | Hz | PWM switching frequency |
| DC Link Voltage | `Vdc` | 400 | V | DC output voltage |
| Input Phase Voltage | `Vin_rms` | 230 | V | RMS input phase voltage |
| Load Resistance | `Rload` | 10 | Ω | Load resistance |
| Filter Inductance | `Lfilter` | 1e-3 | H | Input filter inductance |
| Filter Capacitance | `Cfilter` | 100e-6 | F | Input filter capacitance |

### Derived Parameters

- **Input Line Voltage**: `Vline = Vin_rms × √3`
- **Modulation Index**: `m = Vdc / Vphase`
- **DC Link Current**: `Idc = Vline / (√3 × Rload)`

## 📈 Results

The simulation generates the following outputs:

### Console Output
- Complete parameter summary
- Calculated derived parameters
- Performance metrics including:
  - Average, maximum, and minimum output power
  - RMS input current values

### Graphical Output
1. **PWM Signals Plot**: Three-phase PWM waveforms
2. **Input Phase Current**: Sinusoidal current waveform
3. **Output Power**: Power variation over time

## 📁 Project Structure

```
pwm-rectifier-analysis/
├── README.md
├── pwm_rectifier_analysis.m    # Main simulation script
├── docs/
│   ├── project_report.pdf      # Detailed project report
│   └── code_documentation.pdf  # Code explanations
├── results/
│   ├── sample_output.png       # Example simulation results
│   └── performance_data.mat    # Saved simulation data
└── LICENSE
```

## 📊 Performance Metrics

The simulation calculates and displays:

- **Average Output Power**: Mean power delivered to the load
- **Maximum Output Power**: Peak power during operation
- **Minimum Output Power**: Minimum power during operation
- **RMS Input Current**: Root mean square of input phase current

## 🔮 Future Enhancements

- [ ] **Multi-level PWM implementation**
- [ ] **Harmonic analysis capabilities**
- [ ] **Efficiency calculation modules**
- [ ] **Advanced filtering techniques**
- [ ] **Real-time parameter adjustment GUI**
- [ ] **Comparative analysis with different rectifier topologies**
- [ ] **Export functionality for results**

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 👥 Authors

- **Eman Arshad** - *Initial work and implementation*
- **Abubakar Zubair** - *Code development and testing*
- **Ahmed Shah** - *Documentation and analysis*

**Class**: BSCE-4  
**Course**: Signals and Systems Lab  
**Supervisor**: Mam Shahinza

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Special thanks to **Mam Shahinza** for supervision and guidance
- KICSIT for providing the academic environment
- ResearchGate community for reference materials

## 📞 Contact

For questions or support, please contact:

- **Email**: your.email@example.com
- **Institution**: KICSIT
- **Project Repository**: [GitHub Link](https://github.com/yourusername/pwm-rectifier-analysis)

---

**Note**: This project is part of an academic assignment for the Signals and Systems Lab course. The simulation provides educational insights into PWM rectifier behavior and is suitable for learning purposes in power electronics.
