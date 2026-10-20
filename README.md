# gratuity-valuation-model
Illustrative gratuity valuation using the projected unit credit method (Python and Excel, synthetic data).
Illustrative Gratuity Valuation: Summary of Results
From: Paras Gulati  |  Date: October 2026  |  Valuation date: 31 March 2026
This is a learning exercise using synthetic (randomly generated) employee data and illustrative assumptions. It is not a valuation of any real organisation.
Purpose
To estimate the gratuity liability for a synthetic group of 150 employees, using the projected unit credit method that Ind AS 19 uses for defined benefit obligations, and to show what drives the result.
Method in brief
Gratuity is paid when an employee leaves, at 15 days' wages for each completed year of service: (15 ÷ 26) × monthly wages × years, with a part-year over six months counted as a full year, a five-year service requirement for most exits, and a ceiling of ₹20 lakh. For each employee, I projected wages and the benefit at every possible exit year, weighted each by the probability of leaving in that year, kept only the share of the benefit earned by the valuation date, and discounted it to that date. The total across employees is the Defined Benefit Obligation (DBO).
Key results
• DBO: ₹4.68 crore (₹4,67,85,528)
• Current service cost, next year: ₹37.2 lakh
• Interest cost, next year (approximate): ₹32.7 lakh
• Expected payments in year 1 for service earned to date: ₹39.9 lakh
• Weighted average term of the liability: 8.7 years
• Employees: 150, of whom 100 already have five or more years of service
What the results show
• The DBO is about 60% of the ₹7.84 crore that would be owed if every eligible employee left today. Discounting and counting only service earned so far outweigh the effect of wage growth.
• The group is young (average age 38), but the liability falls due much sooner than retirement, because most employees are expected to leave before 60.
• The liability is concentrated: the top 10 employees account for 22.8% of the DBO.
Assumptions
• Discount rate: 7.0%, a proxy for the 10-year government bond yield around the valuation date (approximate)
• Salary escalation: 8.0% a year (illustrative)
• Retirement age: 60
• Ceiling: ₹20 lakh (to be verified against the current notification)
• Mortality and withdrawal: illustrative placeholders, not published or company-specific rates
Checks performed
The valuation function reproduces a hand-calculated example exactly. The same valuation was built separately in Python and in Excel, and the two agree on every headline figure and on every employee's DBO. The cash flows, once discounted, reconcile to the DBO.
Limitations
• Synthetic data and placeholder assumptions: results show the method, not a real liability.
• Exits are treated as happening at the end of whole years, and ages are rounded down.
• The ceiling is applied to the projected benefit before attributing it to service, which simplifies Ind AS 19.
• Interest cost is approximated as the discount rate times the opening DBO.
• Fixed-term employees and plan assets are not modelled.

