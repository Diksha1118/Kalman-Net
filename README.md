Preprint: https://www.biorxiv.org/content/10.1101/2024.10.03.616126v1

**Prediction of Monkey Limb Movements via the Neural Data**

#X_1 for X pos and X_2 for Y pos
#X_3 for velocity X pos, X_4 for velocity Y pos
5:95>>>> Channel data

KalmanNet is the integration of deep learning and Kalman filtering to decode motor intent from neural time-series data for brain-machine interface (BMI) systems. Training the trajectory and the observation models on the training data & predicting the gain, i.e., the metric of trust in the observations, from the deep learning model and using it to calculate the current state. This enables dynamic trust modulation, where KalmanNet relies more on neural signals for initiating movement but trusts
dynamical models for stopping movements, improving safety.

Conducted performance benchmarking between KalmanNet, LSTM, and traditional Kalman filters across metrics like position & velocity correlation and task success rate using rigorous statistical tests (e.g., paired t-tests, p < 1e-7).

KalmanNet performed comparably or better than deep-learning models in both offline (pre-recorded data) and online (real-time) settings. In offline trials (13 days, 2 monkeys), KalmanNet’s velocity correlation was similar to LSTM (p = 0.64) and significantly better than standard Kalman filters (p < 1e-7). In online trials (real-time BMI control), KalmanNet had a higher success rate (97%) than LSTM (90%), despite LSTM achieving faster movement execution.



