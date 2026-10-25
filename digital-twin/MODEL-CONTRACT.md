# Proposed model contract

## Purpose and boundary

Explain which combinations of location, population, enterprise, infrastructure, financing, ownership, and services can produce worthwhile household outcomes, under what assumptions and risks. Define one node and its outside relationships before modeling a national network.

## Entities and state

Use explicit enterprises, households, community entities, government, infrastructure assets, land parcels, outside markets, and finance providers. Track households and recipients separately. State includes cash, debt, fund assets, housing capacity and condition, occupied parcels, infrastructure capacity, and constrained resources.

| Domain | Minimum input / state | Output and consistency question |
| --- | --- | --- |
| People | Household composition, work, income, care needs, arrival and exit | Who benefits or loses, and how does the denominator change? |
| Land and homes | Developable land, tenure, unit costs, construction and maintenance | Can promised occupancy physically and legally occur? |
| Money | Entity cash, contracts, ownership, finance, prices and taxes | Do accounts reconcile without hidden funding or duplicate benefits? |
| Enterprise | Paying demand, production, sales, costs, staffing, reinvestment | What real income enters the node and what cash reaches each owner? |
| Water | Available and permitted supply, storage, quality, demand | Does seasonal and stressed demand exceed usable supply? |
| Energy | Loads, generation, storage, grid access, losses and backup | Are peaks, energy balances, costs, and outages represented? |
| Food and logistics | Crop output, procurement, spoilage, transport capacity | Are goods available at the modeled total cost? |
| Services | Health, education, care, transport and administrative capacity | Do access and service promises exceed staff or capacity? |
| Technology | Readiness, deployment delay, downtime, supervision | Does the case still work without speculative capability? |

## Time, behavior, and uncertainty

Begin with an annual financial skeleton and explicit startup timing. Couple it to finer energy, water, and service-capacity calculations where annual averages conceal failure. Do not infer hourly reliability from annual generation totals.

Use transparent behavioral rules and synthetic households. Separate empirically grounded behavior from speculative responses. When stochastic behavior is implemented, save model version, input version, random seed, and run configuration. Compare distributions and sensitivity, not just a single favorable run.

## Validation layers

1. **Bookkeeping:** conserved money transfers, assets/debt movements, resource balance, consistent units and denominators.
2. **Component checks:** compare costs, yields, loads, and service rates against source evidence and simple hand calculations.
3. **Empirical calibration:** compare defined components with actual analogous communities or operating systems; reserve evidence for out-of-sample checks where feasible.
4. **Decision usefulness:** show whether the recommendation changes under plausible input ranges, alternative behavioral rules, and coupled failures.

Publish failures and uncertainty. A passing bookkeeping suite satisfies only layer 1. Do not call the whole model validated because internal identities balance.

## Visual and explanation requirements

The bird's-eye landscape should reflect modeled land use, homes, infrastructure, and activity. Household views should reconcile with the same accounting engine. Every prominent metric should show unit, period, denominator, source/assumption, and the mechanism behind changes. Let a viewer compare scenarios and inspect startup costs, debt, resource limits, and downside outcomes as easily as dividends or growth.

## First implementation decision still open

No new language, framework, simulation engine, hosting platform, data service, or paid dependency is selected by this foundation. Audit the existing prototype and define a bounded model task before selecting the implementation. Keep the model runnable independently of the visual frontend where practical.
