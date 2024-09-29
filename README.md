java c
Problem Set 2
Applied Econ 440.602: Macroeconomic Theory
Fall, 2024
1. Accommodating Technical Change. Consider an economy with linear consumption and investment functions:
C = c0 + c1 × Y                                      (1)
I = b0 + b1 × Y − b2 × r.                         (2)
Assume that the parameters c0, c1, b0, b1, and b2 are all positive, and that c1+b2 < 1. For the purposes of this question, we’ll ignore fiscal policy, which is why there are no taxes in the consumption function. Without fiscal policy, the aggregate demand identity reduces to:
Z = C + I,                                      (3)
and the equilibrium condition remains Z = Y . Monetary policy is summarized by the LM curve:
r = ¯r,                                      (4)
where ¯r is the interest rate by the central bank, which we’ll treat as exogenous. Suppose that there’s a technological innovation that makes it easier for firms to produce more output for a given amount of inputs. We’ll be modeling this technological innovation as an increase in the autonomous component of investment from b0 to b'0 > b0.
(a) Holding all else fixed, what is the effect of the technological innovation on the IS curve? Explain your reasoning.
(b) Let’s consider the market for money, and how the central bank behaves in the wake of the techno-logical change. Assume that prices are completely sticky, so the real interest rate and the nominal interest rate are the same.
i. Holding all else fixed, does the technological change cause the demand curve for money to move outward, move inward, or remain fixed? Explain your reasoning.
ii. Suppose that the central bank keeps ¯r fixed following the technological change. That does not mean that the central bank does nothing. In particular, in the supply-and-demand model of the market for money, what does the central bank need to adjust following the technological change? Draw a supply-and-demand graph, and explain your reasoning.
2. Balanced-Budget Multipliers. Consider an economy where the IS and LM curves are given by:
IS: Y = C (Y − T) + I (Y, r) + G                                   (5)
LM: r = ¯r,                                                                (6)
where ¯r is the interest rate by the central bank, which we’ll treat as exogenous. Otherwise, the notation is the same as what we introduced in class. The consumption function C (·) is increasing, and the investment function I (·, ·) is increasing in its first argument and decreasing in its second argument. Assume that, initially, the government is running a balanced budget, meaning that T = G.
(a) Assume that 0 < C′(YD) < 1 for any level of disposable income YD. Explain, in words, the economic meaning of this assumption.
(b) To ensure that an equilibrium exists in the market for goods, what additional assumptions do you have to make about the derivatives of the consumption and investment functions? Explain your reasoning.
(c) Consider a proposal for the government to abandon its balanced budget and engage in deficit spending. That is, G goes up, but T remains fixed at its initial level.
i. Derive an expression for the government-spending multiplier dG/dY.
ii. Is this government-spending multiplier positive, negative, or zero? Explain how you know mathematically.
iii. Is this government-spending multiplier greater than, less than, or equal to one in absolute value? Explain how you know mathematically.
(d) Consider a proposal to expand government spending, while maintaining a balanced budget G = T. That is, G goes up, and T is simultaneously adjusted to increase dollar-for-dollar with G.
i. Derive an expression for the government-spending multiplier dG/dY.
ii. Is this government-spending multiplier positive, negative, or zero? Explain how you know mathematically.
iii. Is this 代 写Econ 440.602: Macroeconomic Theory Problem Set 2 Fall, 2024Matlab
代做程序编程语言government-spending multiplier greater than, less than, or equal to one in absolute value? Explain how you know mathematically.
(e) Now, let’s compare the above two proposals. Which one will result in a larger change in output? Explain how you know mathematically, and provide a brief economic explanation in words.
3. Exploring Okun’s Law. The relationship between real output and unemployment is known as Okun’s law. There are several versions of Okun’s law, and this exercise will have you explore them empirically. Start off by going to FRED to get the following data: unemployment (UNRATE) and real GDP (GDPC1). The raw unemployment data is monthly, but we’ll have to make it quarterly to match the GDP data. When you pull up the unemployment data in FRED, click on “Edit Graph,” go to “Modify Frequency,” and select “Quarterly,” with aggregation method “End of Period.” Your sample for the variables should run from 1947 to 2024. Throughout, Let ut denote the unemployment rate at date t, let Yt denote real GDP at date t, and let %∆Yt ≡ (Yt − Yt−1) /Yt−1 denote the GDP growth rate at date t.
(a) The version of Okun’s law presented in Blanchard says that the growth rate of output %∆Yt is systematically related to the change in unemployment ∆ut ≡ ut − ut−1.
i. Construct two scatter plots with %∆Yt on the horizontal axis and ∆ut on the vertical axis. For the first plot, use only data from 1947 to 2019. For the second plot, use the full sample from 1947 to present.
ii. Using the 1947–2019 sample, compute the correlation coefficient between %∆Yt and ∆ut.
iii. Using the 1947–2019 sample, estimate the regression:
%∆Yt = β0 + β1 × ∆ut + ϵt,                          (7)
where ϵt is a residual. What is the estimated value of β1?
(b) Some economists prefer to look at how deviations from trend in GDP are related to deviations from trend in unemployment. To do so, it’s necessary to specify what, exactly, we mean by trend. We’ll use the Hodrick-Prescott (HP) filter. For any variable xt, the HP trend τt is the solution to the following minimization problem:

where λ > 0 is a parameter that controls how smooth the trend is. Notice that the first sum is minimized by setting τt = xt, and the second sum is minimized by a linear trend (by setting ∆τt equal to a constant). Hence, a low value of λ produces a more flexible trend that closely tracks all the fluctuations in the data, and a high value of λ produces a more rigid trend that’s closer to a straight line. When working with quarterly data, it’s standard practice to set λ = 1, 600, and that’s what you should do when applying the HP filter in this exercise. In Stata, you can compute the HP trend using the command tsfilter hp. In MATLAB, you can compute the HP trend using the command hpfilter. (You can also download an add-in for Microsoft Excel that will compute the HP filter, but I encourage you to do the exercise using a statistical or mathematical coding language.)
i. Let τt(u)denote the HP trend of ut. Let u*t ≡ ut −τt(u)denote the deviation in unemployment from the HP trend. Plot u∗t over the sample from 1947–2024.
ii. Let τt(y)denote the HP trend of log (Yt), where log (·) to denotes the natural logarithm. Let yt* ≡ 100 ×h log (Yt) − τt(y)idenote the deviation in log GDP from the HP trend, multiplied by 100. (By looking at the log deviation times 100, we can interpret yt* as the approximate percent deviation from trend in real GDP.) Plot yt* over the sample from 1947–2024.
iii. Construct a scatter plot with yt* on the horizontal axis and u*t on the vertical axis.
iv. What is the correlation coefficient between yt* and u*t?
v. Estimate the regression:
yt* = β0 + β1 × u*t + ϵt,                     (9)
where ϵt is a residual. What is the estimated value of β1?









         
加QQ：99515681  WX：codinghelp
