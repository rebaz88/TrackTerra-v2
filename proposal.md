# Grant Proposal: Funding for TrackTerra

- **Project Name:** TrackTerra
- **Team Name:** TrackTerra
- **Payment Address:** terra17g2kuc9xrcdmhh660mwcus7fxkcefue7zlsa6p

## Project Overview

As you might already know TrackTerra is a tax and reporting application. It is build to ease the process of transforming the blocks/transactions data into a single transaction form similar to traditional banking systems. It currently supports native send/recieve, anchor, mirror(partially), pylon(partialy) and terraswap protocols.

### Overview

- TrackTerra – a tax focused blockchain explorer for Terra
- TrackTerra parsers transactions from terra wallets in to a format that can easily be imported in to popular crypto tax software.
- Removes the complexity and barrier to entry around reporting requirements for transactions in the terra ecosystem

### Project Details

The app uses nodejs and has it’s own database backend where it stored parsed transactions. Our MVP is mostly functional and can be demoed at beta.trackterra.org. Active development can be viewed [here](https://github.com/rebaz88/TrackTerra-v2/)

### Ecosystem Fit

- The target end users are users of the terra ecosystem that have any sort of tax reporting requirement, and crypto tax softwares that will either adopt our codebase or use our APIs. Crypto tax reporting is a major burden for crypto investors and this solution aims to solve this for the terra ecosystem.
- There is one competitor to trackterra which is stake.tax, however this solution is nearly unusable and doesn’t have support for many terra transactions. This solution is also not opensource. TrackTerra aims to build a solution that can easily be extended with little development effort that is also fully opensource.

## Team

### Team members

- Papi - Project Manager
- Rebaz Saleh - Software Developer

### Contact

- **Contact Name:** Papi
- **Contact Email:** trackterraorg@gmail.com
- **Website:** beta.trackterra.org

### Legal Structure

- N/A

### Team Code Repos

- https://github.com/Papi94/TrackTerra-v2
- [https://github.com/Papi94](https://github.com/Papi94)
- [https://github.com/rebaz88](https://github.com/rebaz88)

### Overview

- **Total Estimated Duration:** 50 working days
- **Full-Time Equivalent (FTE):** 1 FTE
- **Total Costs:** 38,800 USD

### Milestone 1  — **Add support for dynamically adding new protocols**

- **Estimated duration:** 40 working days
- **FTE:** 1
- **Costs:** 22,400 USD

| Number   | Deliverable | Specification      |
| :---------- | :------------ | :------------|
| 1           | Generic Classifier & Parser       |   - Create a scrapper to go through each protocols transactions and store them in a database for later use <br> - Classify the transactions Manually/Automatically and add support for each transaction type in the current version <br> - Write test for each transaction type for each protocol. <br> - Develop a generic classifier that is able to classify all types of the transaction for each protocol. <br> - Write test for the generic classifier. <br> - Add parser for some of the transactions that are not parsed by the current parser. <br> - Write test for each parser. <br> - Develop a generic parser that is able to parse all the transaction types for each protocol. <br> - Write test for the generic parser.|
| 2           | Add ui for managing protocols & transaction types       | - Add ability to add rules for each protocol/transaction type through ui. <br> Write unit and e2e test for adding rules through ui <br> Protect ui to allow only authenticated users to add protocols/transaction types.       |
| 3           | Supporting protocols       | Minimal Support: Anchor, Mirror, Terraswap, Nexus, Valkyre, Mars, Astroport, Loop, Spectrum, Apollo|

<br>

### Milestone 2  — **Add support for tax software**

- **Estimated Duration:** 5 working days
- **FTE:** 1
- **Costs:** 3,200 USD

| Number   | Deliverable | Specification      |
| :---------- | :------------ | :------------|
| 1           | Export data to a format readable by Koinly , Cointracker       |  - Users will be able to filter the transaction by date, transaction type. <br> - Users will be able to export the data to three supported third-pary apps based on their filter.|

<br>

### Milestone 3 — **Add support for REST and GraphQL**

- **Estimated Duration:** 5 working days
- **FTE:** 1
- **Costs:** 3,200 USD

| Number   | Deliverable | Specification      |
| :---------- | :------------ | :------------|
| 1           | This will allow interacting with the application for third-party apps       |  Retrieve and filter data by  Wallet address, Transaction type, Transaction date  |

<br>

### Maintenance and Upkeep

- **Duration:** 1 Year
- **FTE:** 1
- **Costs:** 10,000 USD

| Number   | Deliverable | Specification      |
| :---------- | :------------ | :------------|
| 1           | Maintain the application       |  Bug fixes and new small features that would improve the overal usability/performance of the application  |
| 2           | Hosting the application      |  Cover the costs associated with hosting the application. (excluding FCD)  |
<br>

### NFT Marketplace support
Adding support for NFT marketplace is among our stretch goals. If we did not get to this goal, we will tap in to upkeep fund to cover those development costs