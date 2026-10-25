# Accounting contract for future models

**Status: proposed modeling requirements. No operating budgets have been established.**

## Boundaries and entities

Define the node boundary, year, price basis, time step, resident population, households, workers, and eligible recipients. Represent operating enterprises, utility operators, developers/landholders, resident investment vehicles, local government, households, outside customers, lenders, and external investors separately where they have different rights or obligations.

## Keep the flows explicit

1. Enterprise sales pay for inputs, labor, taxes, financing, maintenance, reinvestment, and changes in working capital before any eligible owner distribution.
2. A community entity receives only the cash its documented rights provide. Ownership percentage, voting power, and cash entitlement may differ.
3. Community cash pays its own obligations, service benefits, administration, reserves, and approved investment before a residual household payment is considered.
4. Households receive wages, remote income, pensions or transfers, hosting payments, and ownership distributions. They pay the complete stated budget of essentials, taxes, fees, debt service, and other required costs.
5. Government taxes and spending have their own authority and budget. A private discount or trust payment is not a tax reduction.

Use a consistent definition of enterprise cash eligible for distribution. If debt service, maintenance, tax, or working capital has already been deducted, do not deduct it twice. If a source reports an accounting margin instead, build the bridge to cash explicitly.

## Minimum relationships

```text
enterprise_cash_available = receipts - cash_operating_costs - taxes
                            - debt_service - required_capital_spending
                            - increase_in_working_capital - required_reserve_additions

community_receipts = contractual_cash_entitlements + rents + net_utility_distributions
                     + other_defined_receipts

community_residual = community_receipts - community_obligations - service_benefit_spending
                     - community_investment - community_reserve_additions

monthly_payment = max(0, permitted_distribution) / eligible_recipients / 12

household_cushion = household_cash_income - defined_essential_outlays
                   - taxes_and_required_fees - debt_service
```

Adjust these identities to the financing structure and time step; document the change. A negative residual requires a stated funding source, reduced spending, or default/failure behavior. It must not vanish through clipping. Fund withdrawals are a source only while assets and rules permit them.

## Avoid duplicate benefits

If a crop host is paid, the enterprise pays that cost. If a household gets a grocery benefit, identify the payer and the food budget. If wages are counted in household income, they remain enterprise costs. If a utility's surplus is distributed, do not also treat it as retained capital. Reduced bills can improve household outcomes without creating distributable cash for another entity.

Transfers within the node cancel in a consolidated cash view. Outside earned income, transfers, financing, and asset sales should be distinguishable. Keep total sales separate from value added. Local recirculation can matter for activity but is not a new external funding source every time money changes hands.

## Required comparisons

Show startup, first occupancy, stabilized operation, growth, downturn, and replacement years. Include zero-dividend, delayed anchor, higher financing cost, lower automation, and constrained-resource cases. Report median and low-income cohort outcomes, renters and owners, older residents, caregivers, people unable to work, and newcomers. Distinguish pre-tax and after-tax outcomes.

Report affordable essentials and household cushion separately. A payment that is absorbed by rent or fees may leave the household no better off. Do not infer happiness or public acceptance from an aggregate financial surplus.
