# Bank Term Deposit Predictive Machine Learning Model
-> To check all the coding and analysis of this project, just click on the Jupyter Notebook above!

## Brief Overview

### Project Development
This project was developed locally with Visual Studio Code and GitHub version control.

Please check this project @ [GitHub page](https://caiocvelasco.github.io/) or @ [GitHub Repository](https://github.com/caiocvelasco/ml-project-bank-term-deposit/blob/4f1bfa72d17cefdfe2a515054f1f2cfffa3c7749/bank-term-deposit-notebook.ipynb).

### Problem Definition

A bank would like to understand the main factors driving customers to subscribe a Term Deposit.

### Objective
Our goal is to build a classifier (supervised machine Learning model) to predict whether customers would subscribe a Term Deposit. In case we find high accuracy in our model, it would imply that the bank marketing department could benefit from an efficient use of available resources by focusing on the "right" customers (given by our _classifier_). Moreover, we want to understand which other factors might also affect customers' decision.

* Recall: Classification Model

    The goal of a classification model is to build a data-driven model that learns an unknown underlying function that maps several input variables, which characterize an item (e.g., bank client, with one labeled output target (e.g., type of bank deposit sell: “failure” or “success”). 
    _[Moro et al., 2014] S. Moro, P. Cortez and P. Rita. A Data-Driven Approach to Predict the Success of Bank Telemarketing. Decision Support Systems, Elsevier, 62:22-31, June 2014_

### Field Knowledge

Suppose a bank is interested in predicting whether its customers would subscribe a _Bank Term Deposit_. 

**What is a term deposit and why does someone want to invest their money?**

Before answering these questions, let's look into some important definitions and then into some insights from Economic Theory. This will help understand the scenario.

**Financial Instruments**

A financial instrument is an asset that can be traded between entities. An agreement (or contract) will hold both parties accountable for such transaction.
We can divide financial instruments into different classes of financial instruments. An example is the _Debt-Based Financial Instruments_.

**Debt-Based Financial Instruments**

The term _debt_ comes from the fact that some financial institutions want to raise capital by borrowing money from people. When this transaction happens, the financial institution has the obligation to pay back at a later date, with interest. Thus, the financial institution has a _debt_ with the lender.
Such instruments can also be interpreted as a _Certificate of Deposit_, i.e., you _deposit_ money into an account at a financial institution for some period of time in exchange for future compensation.

**Maturity**

Maturity is the period of time it takes for the lender to withdraw this or her money from the bank. Maturity date is the agreed-upon date on which the investment ends.

**Fixed-term Investment**

When a financial instrument has a fixed time period of investment, the maturity is known at the time of issuance and the lender cannot withdraw its money befeore maturity without incurring on a _early withdrawal penalty_. This penalty is important to the bank, because a bank makes money by lending its customers deposits to other entities and profiting on top of that. Banks need to reduce risk in their operations and such penalties account for the unexpected costs created by customers who decide to withdraw their deposits before maturity.  

**Term Deposit**

Term Deposit is an example of a _Fixed-Term, Debt-Based Financial Instrument_, also called a _Certificate of Deposit_.
Moreover, a Term Deposit is a risk-free investment since they are backed by the government.
In sum:
* When a customer subscribes to a **Term Deposit** he or she will deposit (or invest) money into a bank account, agreeing not to withdraw their funds for a fixed period in return for future compensation (interest), i.e., before maturity.

**The Decision Problem faced by an Investor**

An investor is an individual (or entity) who makes certain decisions regarding how he or she spends his or her money.
* How much of my money should I use in consumption (goods or services) now?
* From what is left, how much should I spend on investment opportunities?

Such decisions are unscapable to the individual because resourses are limited. You only have a certain amount of money and you need to make decisions regarding how to spend it.
We say that the investor faces a _trade-off_ between consuming less now to (hopefully) consume more in the future, i.e.:
* Spend less in consumption at the beginning of a period in exchange for an investment opportunity that will hopefully earn profits at the end of the period.

**Economic Incentives behind Consumer Behavior & Investment Opportunities**

An _Economic Incentive_ is something that motivates or drives one to behave in a certain way. The most simple example in Economics is: Prices.\
_Prices_ provide an incentive mechanism that might induce people's behavior in a certain way. For example, if the price of apples go up, you will probably buy less apples (and buy more of some other good or service).

Good things to know:
* In periods of rising interest rates in society (usually started by the Central Bank), consumers are more likely to invest because it is better to lend money to the bank than to spend it on consumption now. Thus, when the interest rate is higher, people tend to invest more, hence changing their status-quo behavior. Thus, future expectations of _higher interest rates_ could help predict consumer behavior towards subscribing to **Term Deposits**.
* **Term deposits** do not keep up with inflation. If the rate on a term deposit is 3% and the inflation rate. is 3.5%, the customer is not earning enough to compensate for price increases in the economy. Thus, _Inflation Rate_ maybe a strong underlying _economic incentive_ that could help predict consumer behavior towards subscribing to **Term Deposits**.
