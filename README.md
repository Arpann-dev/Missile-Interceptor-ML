# 🛡️ Missile Interceptor - ML Based Prediction System

This project demonstrates a machine learning and physics-based approach to simulate incoming missile trajectories and evaluate whether an interceptor missile (launched from the origin) can intercept it in time.

---

## 📂 Project Files

| File | Description |
|------|-------------|
| `MissileDatGen.ipynb` | Notebook to generate synthetic missile trajectory data using projectile motion equations. |
| `missile_trajectory_dataset_with_both_angles.csv` | Generated dataset with 10,000 samples (impact point and time). |
| `MissileInterceptor.ipynb` | Trains a model, makes predictions, and checks whether interception is feasible. |
| `interceptor_results.csv` | Stores predicted impact locations, times, and whether each interception was possible. |

---

## 🔧 How It Works

- **Missile Data Generation**
  - Simulates launches from left and right angles (20°–70° and 110°–160°).
  - Captures initial velocity, launch position, impact time and location.

- **Machine Learning Prediction**
  - Trains a Random Forest model to predict:
    - `x_impact` – where the missile will land
    - `t_impact` – when the missile will land

- **Interception Evaluation**
  - Calculates if the interceptor can reach the target on time.
  - Conditions:
    - Must start from (0,0)
    - Has a fixed setup time and velocity
    - Interception is possible if it can reach before the missile lands

- **Success Rate Visualization**
  - A pie chart shows how many missiles could be intercepted vs those that couldn’t.

---

## 📊 Example Output

- Pie Chart: Interception vs. Failure
- ~90% Interception Rate (based on simulation parameters)

---

## 🔍 Use Cases

- Defense system simulation
- Predictive target interception
- AI-supported response modeling

---

## 🧠 Technologies Used

- Python
- NumPy, Pandas
- Scikit-learn
- Matplotlib
- Jupyter Notebooks

---

## 🧪 How to Run

> You can run the notebooks in Google Colab or Jupyter Notebook.

1. Open `MissileDatGen.ipynb` → Run to generate dataset
2. Open `MissileInterceptor.ipynb` → Run to train, predict, and evaluate

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙋 Author

Developed by [Arpan Maitra]  
Connect with me on [LinkedIn](https://www.linkedin.com/in/arpan-maitra-424a74295/)


