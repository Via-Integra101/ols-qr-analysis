# OLS QR Decomposition - Interactive Analysis

🔬 **Interactive web app for debugging scientific computing algorithms**

[![Live Demo](https://img.shields.io/badge/Demo-Live-brightgreen)](https://your-username.github.io/ols-qr-analysis)
[![GitHub Pages](https://img.shields.io/badge/Hosted%20on-GitHub%20Pages-blue)](https://pages.github.com/)
[![No Backend](https://img.shields.io/badge/Backend-None%20Required-orange)](https://github.com/your-username/ols-qr-analysis)

## ✨ Features

- **🚀 Pure JavaScript** - Runs entirely in browser, no server needed
- **📊 Interactive Plots** - Real-time Plotly visualizations  
- **🔧 Adjustable Parameters** - Sample size, noise level, random seed
- **📱 Mobile Responsive** - Works on any device
- **🎯 Educational** - Shows algorithm steps and variable inspection
- **🔗 Shareable** - Send the URL to anyone, instantly usable

## 🎮 Try It Live

**👉 [Open Interactive Demo]([https://your-username.github.io/ols-qr-analysis](https://via-integra101.github.io/ols-qr-analysis/))**

## 🚀 Deploy Your Own (2 minutes)

1. **Fork this repo** (click Fork button above)
2. **Enable Pages**: Go to Settings → Pages → Source: "Deploy from a branch" → Branch: "main"
3. **Done!** Your app is live at: `https://your-username.github.io/ols-qr-analysis`

## 💡 Use Cases

- **Algorithm Development**: Visualize data flow and results
- **Teaching**: Interactive demonstrations of OLS concepts
- **Debugging**: Spot-check scientific computing functions
- **Sharing**: Send colleagues a working analysis tool

## 🔧 How It Works

The app implements OLS regression using QR decomposition entirely in JavaScript:

```javascript
function olsQR(X, y) {
    const X_ = addIntercept(X);           // Add intercept column
    const { Q, R } = qrDecomposition(X_); // QR decomposition  
    const beta = solveTriangular(R, Qty); // Solve R*beta = Q^T*y
    const y_hat = matrixMultiply(X_, beta); // Predictions
    const r2 = calculateR2(y, y_hat);      // R-squared
    return { beta, y_hat, r2 };
}
```

## 📊 What You'll See

- **Actual vs Predicted** scatter plot
- **Residuals analysis** for model validation  
- **Residual distribution** histogram
- **Coefficient visualization** with true vs estimated values
- **Real-time metrics**: R², RMSE, sample size

## 🛠 Customize

Fork and modify for your own algorithms:

- Replace `olsQR()` with your function
- Update the plotting logic
- Add new parameter controls
- Extend with more visualizations

## 📝 Perfect For

- **Reddit demos** - Share working code instantly
- **Scientific computing education** 
- **Algorithm validation**
- **Interactive documentation**

---

**No installation, no setup, just share the URL! 🎉**
