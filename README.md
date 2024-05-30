# Capital Expenditure Management

## Scenario

Bluejay Natural Gas is a large energy company based out of Baltimore, MD. The company offers a wide range of energy products and has annual revenues of approximately $50 billion. Because of the diverse nature of the company, its Manager for Project Development, Julie Kavoli, is under continual pressure to manage project proposals from the functional areas of the company. At any point in time, there might be dozens of projects at various stages requiring a wide variety of capital expenditures, promising widely varying future revenue streams, and containing varying degrees of risk. Julie has a difficult balancing act. The company's CEO, Cordelia Kareeni, is very concerned about keeping capital expenditures within a fixed budget and managing risk. The heads of the company's functional areas are less worried about budgets and risks; they are most concerned that their pet projects are approved. Julie also knows that many of the proposed projects, especially those requiring large capital expenditures, must be led by senior project managers with the appropriate experience and skills, and she is keenly aware that the company has only a limited supply of such managers. 

Julie is currently preparing to meet with all parties involved to discuss project proposals for the next three years. She has proposals from the various functional areas for projects they would like to undertake. Each of these is accompanied by a schedule of capital expenditures over the next three years and a financial analysis of the expected revenue streams. These lead to a net present value (NPV) for each proposal, using the company's discount rate of 12%.

Several of the projects, if approved, must be undertaken in joint partnership with another company. For example, if project 3 is approved, Bluejay Natural Gas will take a 50% share in the project, and the other 50% will be shared by a partner.  In this case, Bluejay Natural Gas will only incur 50% of the expenditures and receive only 50% of the revenues.  

## Model Implementation Checklist

Let us create a checklist to address the above problem.

- [ ] **List of given financial information for all potential projects**
  - Ensure the model lists all necessary financial data such as Project Index, Functional Area, Partnership Percentage, Capex for Year 1 to Year 3, and NPV.

- [ ] **Associate each proposed project with an approval indicator**
  - Add a column in the model to indicate whether a project is approved (1) or not approved (0). For now, use random values to simulate scenarios.

- [ ] **Track number of approved projects per functional area**
  - Calculate the number of approved projects for each functional area.
  - Ensure that no functional area is completely shut out of approvals. Use a binary indicator (0 if no projects are approved in the functional area, 1 if at least one is approved).

- [ ] **Calculate the sum of capital expenditures for approved projects**
  - Find the sum of capital expenditures for all approved projects by year and for the total over all three years.
  - Indicate whether these sums exceed the set budget limits using binary values (0 if within budget, 1 if exceeded).

- [ ] **Calculate capital expenditures by functional area**
  - Sum capital expenditures for approved projects, broken down by year for each functional area.

- [ ] **Include a mechanism for adjusting NPV estimates**
  - Allow input for a possible percentage decrease for each project's original NPV.
  - Update the NPV values based on the entered percentage decrease.

- [ ] **Calculate ROI for each project**
  - Implement the calculation of ROI as NPV (adjusted for any decrease) as a percentage of the total capital expenditure of the project.

- [ ] **Create a one-way data table for sensitivity analysis**
  - The table should vary the common percentage decrease in NPV from 0% to 30% in increments of 5%.
  - Outputs should include the average, minimum, and maximum ROI of undertaken projects.

- [ ] **Visual representation of capital expenditures**
  - Develop line charts showing total capital expenditures by year for all approved projects and separately for each functional area.

