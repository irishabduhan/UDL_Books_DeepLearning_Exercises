# Understanding Deep Learning - Exercises & Notes

A comprehensive learning journey through deep learning fundamentals based on the **"Understanding Deep Learning"** textbook by Simon Prince.

📖 **Official Resource:** [https://udlbook.github.io/udlbook/](https://udlbook.github.io/udlbook/)

---

## 📚 Completed Exercises

### **Chapter 2: Supervised Learning**

#### 2.1 Linear Regression ✅
- **File:** `2_1_Supervised_Learning.ipynb`
- **Topics Covered:**
  - 1D linear regression model: f(x) = φ₀ + φ₁·x
  - Loss computation (sum-of-squares)
  - Partial derivatives: ∂L/∂φ₀ and ∂L/∂φ₁
  - Gradient descent optimization
  - Parameter history tracking during training
  - **Loss landscape visualization:**
    - Heatmap showing loss at each (φ₀, φ₁) combination
    - Contour lines for constant-loss regions
    - Gradient descent trajectory (red path)
    - Start point (green circle) and optimal point (red star)
- **Key Learnings:**
  - How to construct a design matrix with bias term
  - Matrix multiplication for batch predictions
  - Computing gradients analytically
  - Effect of learning rate on convergence
  - Visual interpretation of optimization in parameter space

#### Differentiation & Loss Functions (Supporting Work) ✅
- **File:** `differentiation_loss_wrt_parameter.ipynb`
- **Topics Covered:**
  - Design matrix construction: X = [1 | x]
  - Mean Squared Error (MSE) loss function
  - Analytical gradient computation
  - Numerical gradient verification (finite differences)
  - Gradient descent from scratch
  - Loss landscape contour visualization
- **Key Learnings:**
  - Understanding the @ operator (matrix multiplication)
  - Verification: analytical gradients ≈ numerical gradients
  - Convex nature of MSE loss
  - Parameter convergence behavior

---

## 📊 Progress Tracking

| Chapter | Section | Topic | Status | Completion Date |
|---------|---------|-------|--------|-----------------|
| 2 | 2.1 | Linear Regression | ✅ Complete | Nov 30, 2025 |
| 2 | 2.2 | Multivariate Linear Regression | ⏳ Pending | — |
| 2 | 2.3 | Loss Functions | ⏳ Pending | — |
| 3 | 3.1 | Shallow Neural Networks | ⏳ Pending | — |
| 3 | 3.2 | Activation Functions | ⏳ Pending | — |
| 4 | 4.1 | Backpropagation | ⏳ Pending | — |

---

## 🔧 Setup & Requirements

```bash
# Install dependencies
pip install numpy matplotlib scipy

# Run notebooks
jupyter notebook
```

---

## 💡 Key Concepts Learned

### Chapter 2: Supervised Learning
1. **Model Architecture:** Linear model with parameters φ = [φ₀, φ₁]
2. **Loss Functions:** Sum-of-squares and Mean Squared Error
3. **Optimization:** Gradient descent with learning rate α
4. **Gradient Computation:** ∂L/∂φ₀ = (2/m)·Σ(errors), ∂L/∂φ₁ = (2/m)·Σ(errors·x)
5. **Visualization:** Parameter space trajectories on loss landscapes

---

## 📈 Visualization Outputs

### Loss Landscape with Gradient Descent Path
```
- Color intensity: Loss magnitude at each parameter combination
- Gray contours: Constant-loss curves showing optimization region
- Red trajectory: Parameter updates during training iterations
- Green marker: Initial parameter values
- Red star: Converged optimal parameters
```

---

## 📝 Important Notes

- **Learning Rate Selection:** Critical for convergence speed (α = 0.02 works well for this problem)
- **Gradient Verification:** Always verify analytical gradients against numerical gradients
- **Convex Optimization:** MSE loss for linear models is convex → guaranteed global optimum
- **Parameter Initialization:** Started at (φ₀=0.4, φ₁=0.2) or random values
- **Convergence Criterion:** Loss stops decreasing when approaching optimum

---

## 🎯 Next Learning Objectives

- [ ] **Section 2.2:** Multivariate linear regression (multiple input features)
- [ ] **Section 2.3:** Different loss functions (L1, Huber, etc.)
- [ ] **Chapter 3:** Introduction to neural networks and activation functions
- [ ] **Chapter 4:** Backpropagation algorithm and chain rule
- [ ] **Chapter 5:** Deep neural networks and architectures

---

## 📚 Resource Links

- **Official Textbook:** https://udlbook.github.io/udlbook/
- **GitHub Repository:** https://github.com/udlbook/udlbook
- **Chapter 2 (Supervised Learning):** https://udlbook.github.io/udlbook/
- **Code Examples:** Available in official repository

---

## 📊 Overall Progress

```
Completed: 1/15 chapters
Exercises: 2/40+ notebook cells
Estimated Completion: ~8-10 weeks at current pace
```

**Last Updated:** November 30, 2025  
**Current Chapter:** 2 - Supervised Learning  
**Next Focus:** Section 2.2 - Multivariate Regression

---

## 🔍 Debugging & Verification Checklist

✅ Gradient computation verified numerically  
✅ Loss decreases monotonically during training  
✅ Final parameters match expected values  
✅ Visualization shows smooth convergence  
✅ Design matrix constructed correctly  

---

*This learning journey documents progression through "Understanding Deep Learning" with hands-on implementations and visual explanations.*
