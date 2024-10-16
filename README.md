# Position Estimation of Autonomous Vehicle using UKF with XSENSE MTi-G710
This project focuses on the position estimation of an autonomous vehicle using the XSENSE MTi-G710 sensor. Data collected from the sensor is processed using MATLAB, implementing the Unscented Kalman Filter (UKF) algorithm for data fusion, resulting in accurate position estimates.
## Table of Contents
1. Introduction
2. Algorithm
3. Data Collection
4. Installation
5. Usage
6. Results
7. Contributing
8. License
9. Acknowledgements

## Introduction
Accurate localization is essential for autonomous vehicles. This project aims to estimate the vehicle's position by processing data collected from the XSENSE MTi-G710 sensor. The Unscented Kalman Filter (UKF) algorithm is employed to effectively fuse the sensor data and improve position estimation accuracy.

## Algorithm
The Unscented Kalman Filter (UKF) is used for state estimation in nonlinear systems. The following steps outline the process implemented in this project:

1. **Convert LLA to ECEF Coordinates**: Convert initial latitude, longitude, and altitude (LLA) to Earth-Centered, Earth-Fixed (ECEF) coordinates.
2. **Prediction Step**: Use the IMU's accelerometer data for the prediction step, applying the Unscented Transform.
3. **Update Step**: Incorporate GPS latitude and longitude data for the update step.
4. **Convert ECEF to LLA**: Convert the ECEF coordinates back to latitude, longitude, and altitude (LLA).
5. **Display Results**: Display the raw GPS data alongside the filtered data.

## Data Collection
Data was collected using the XSENSE MTi-G710 sensor. Ensure the sensor is properly calibrated and positioned before data collection.

## Installation
1. Install MATLAB and ensure the necessary toolboxes are available.
2. Clone the repository: git clone https://github.com/GSKorimath/Pos_Estimation.git

## Usage
1. Load the collected data into MATLAB.
2. Run the UKF algorithm script: run_ukf_algorithm.mlx
3. View the displayed results and plots.

## Results
The results demonstrate the effectiveness of the UKF algorithm in improving position estimation accuracy. Below are example plots showing the performance of the algorithm.

![image](https://github.com/user-attachments/assets/4162ead0-c6a7-4169-aeac-2d404996464e)


## Contributing
Contributions are welcome! Please open an issue or submit a pull request.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements
Special thanks to [Prof.Rohit Kalyani, Rohit Waddar, Anchal Aravind Patil, KLE Technological University] for their support and contributions to this project.
