# Capital Expenditure Management

## Scenario

Bluejay Natural Gas is a large energy company based out of Baltimore, MD. The company offers a wide range of energy products and has annual revenues of approximately $50 billion. Because of the diverse nature of the company, its Manager for Project Development, Julie Kavoli, is under continual pressure to manage project proposals from the functional areas of the company. At any point in time, there might be dozens of projects at various stages requiring a wide variety of capital expenditures, promising widely varying future revenue streams, and containing varying degrees of risk. Julie has a difficult balancing act. The company's CEO, Cordelia Kareeni, is very concerned about keeping capital expenditures within a fixed budget and managing risk. The heads of the company's functional areas are less worried about budgets and risks; they are most concerned that their pet projects are approved. Julie also knows that many of the proposed projects, especially those requiring large capital expenditures, must be led by senior project managers with the appropriate experience and skills, and she is keenly aware that the company has only a limited supply of such managers. 

Julie is currently preparing to meet with all parties involved to discuss project proposals for the next three years. She has proposals from the various functional areas for projects they would like to undertake. Each of these is accompanied by a schedule of capital expenditures over the next three years and a financial analysis of the expected revenue streams. These lead to a net present value (NPV) for each proposal, using the company's discount rate of 12%.

Several of the projects, if approved, must be undertaken in joint partnership with another company. For example, if project 3 is approved, Bluejay Natural Gas will take a 50% share in the project, and the other 50% will be shared by a partner.  In this case, Bluejay Natural Gas will only incur 50% of the expenditures and receive only 50% of the revenues.  

![Starting Data](https://github.com/adiimated/Capital-Expenditure-Management/blob/main/images/Starting%20Data.png)

## Excel Model Development Steps

1. **List Financial Data**
   - Include all provided financial estimates for potential projects: Project Index, Functional Area, Partnership Percentage, Capex Year 1-3, and NPV.

2. **Project Approval Indicator**
   - Add a column to indicate if each project is approved (1) or not approved (0). Use random values initially to test various scenarios.

3. **Functional Area Approval Tracking**
   - Calculate the total number of approved projects for each functional area.
   - Ensure no functional area is left out by adding a binary indicator (1 if at least one project is approved, 0 otherwise).

4. **Capital Expenditure Calculations**
   - Determine total and yearly capital expenditures for approved projects.
   - Use binary indicators to check if these sums exceed the set budget limits of $10 billion total and $4 billion per year.

5. **Expenditure Breakdown by Functional Area**
   - Calculate and display capital expenditures by year for each functional area based on project approvals.

6. **NPV Adjustments**
   - Allow for input of a percentage decrease to adjust each project's NPV.
   - Update NPV calculations based on the inputted decrease percentage.

7. **ROI Calculation**
   - Compute the ROI for each project using the formula: (Adjusted NPV / Total Capital Expenditure) * 100%.

8. **Sensitivity Analysis**
   - Create a one-way data table that varies the percentage decrease in NPV from 0% to 30% in 5% increments, displaying changes in ROIs.

9. **Visualization of Capital Expenditures**
   - Develop line charts to visualize total and functional area-specific capital expenditures for all approved projects across each year.

## Model:

![](https://github.com/adiimated/Capital-Expenditure-Management/blob/main/images/Modeling%20Data.png)

![](https://github.com/adiimated/Capital-Expenditure-Management/blob/main/images/Conditions%20and%20Viz.png)
