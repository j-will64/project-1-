Affects of Interest rates
Written by Jarrod Williams, Bill Smith, Marc Conwell

Our three main question we wanted to answer with the data we generated are:

Question 1: Is there a liner relationship between short-term interest rates and long-term interest rates? 

Question 2: Is there a liner relationship between short-term interest rates and change in S&P500?

Question 3: Is there a liner relationship between sunspot activity and short-term interest rates? 

The Conclusion are as followed:

Question 1

	Random Variable X = TB3MS = 3-month treasury bill interest rate 
	Random Variable Y = 30YEAR = home mortgage interest rates on a 30-year fixed mortgage
	ASSUME: There is no linear relationship between random variables X and Y
		• Null Hypothesis, H₀ : ρ = 0
		• Alternate Hypothesis, H₁ : ρ ≠ 0
	Correlation Coefficient (X , Y) = ρ = 0.929872 
	T-test statistic = ρ [(n-2 )/(1 – ρ ^ 2)] ^ ½ = 0.93 [ 628 / (1 – 0.93 ^2)] ^ ½ = 23.3 
	2-tail test with α = 0.05 ; n = 630 ; 2 degrees freedom → critical value t-dist = 1.964

	Conclusion:
	• Conclusion: We reject null hypothesis.
	• Data is consistent with linear relation between long term and short-term interest rates.
	• This is exactly what we would expect because interest rates tend to move together.
![image](https://github.com/j-will64/project-1-/assets/53585498/29f1a289-f6f9-4cd4-8198-49c35dae5d9c)



Question 2

	Random Variable X = TB3MS = 3-month treasury bill interest rate 
	Random Variable Y = SP500 = Percent change in SP Index over the month 
	ASSUME: There is no linear relationship between random variables X and Y 
		• Null Hypothesis, H₀ : ρ = 0 
		• Alternate Hypothesis, H₁ : ρ ≠ 0 
	Correlation Coefficient (X , Y) = ρ = -0.02 
	T-test statistic = ρ [(n-2 )/(1 – ρ ^ 2)] ^ ½ = -0.02 [ 628 / (1 – (-0.02 ^2))] ^ ½ = -0.52 
	2-tail test with α = 0.05 ; n = 630 ; 2 degrees freedom → critical value t-dist = 1.964 
	[ T-test statistic = | -0.52| ] < [Critical value = 1.964 ] → WE ACCEPT NULL HYPOTHESIS

	Conclusion 
		• Conclusion: We can not reject null hypothesis. 
		• Data is consistent with NO linear relation btwn short-term interest rates and ∆ SP500. 
		• This was kind of surprising because people say interest rates strongly impact stock market. 
		• Dig deeper and it’s CHANGE in EXPECTIONS for future interest rates that drive stock market 
		• Presumably we’d have strong linear relationship with expected future change in interest rates.


Question 3

Random Variable X = SUNSPOTS = Percent change in sunspots compared to historical average 	Random Variable Y = TB3MS = 3-month treasury bill interest rate 
	ASSUME: There is no linear relationship between random variables X and Y 
		• Null Hypothesis, H₀ : ρ = 0 
		• Alternate Hypothesis, H₁ : ρ ≠ 0 
	Correlation Coefficient (X , Y) = ρ = 0.44 
	T-test statistic = ρ [(n-2 )/(1 – ρ ^ 2)] ^ ½ = -0.02 [ 628 / (1 – 0.44 ^2)] ^ ½ = 12.4 
	2-tail test with α = 0.05 ; n = 630 ; 2 degrees freedom → critical value t-dist = 1.964 
	[ T-test statistic = 12.4 ] > [Critical value = 1.964 ] → WE REJECT NULL HYPOTHESIS

	Conclusion 
		• Conclusion: We reject null hypothesis. 
		• SUNSPOTS CORRELATE To INTEREST RATES !!! 
		• Awesome example of limitations of looking to correlation matrix for significance.


The graphs are stored in the wiki page.

After cloning the repositorie run the code "pip install -r requirements.txt" in the command line of the main folder.
