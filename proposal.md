## PROJECT INTRODUCTION
As you might already know TrackTerra is a tax and reporting application. It is build to ease the process of transforming the blocks/transactions data into a single transaction form similar to traditional banking systems. It currently supports native send/recieve, anchor, mirror(partially), pylon(partialy) protocols. 

## PROPOSAL
This proposal is to further develop the application in order to
- Add support for dynamically adding new protocols
- Add support for different taxing software when exporting the data
- Add support for REST and GraphQL to query the applcation(Limited)

The major activities include redesiging the core functionality of the system which is the indexer to support the addition of new protocols dynamically.

## DEVELOPMENT ROADMAP
* ### **Add support for dynamically adding new protocols**
    * Est. Duration: 40 days
    * Funding: $22,400
    * Procedure:
        <ol>
            <li>Create a scrapper to go through each protocols transactions and store them in a database for later use</li>
            <li>Classify the transactions Manually/Automatically and add support for each transaction type in the current version</li>
            <li>Write test for each transaction type for each protocol.</li>
            <li>Develop a generic classifier that is able to classify all types of the transaction for each protocol.</li>
            <li>Write test for the generic claissifier.</li>
            <li>Add parser for some of the transactions that are not parsed by the current parser.</li>
            <li>Write test for each parser.</li>
            <li>Develop a generic parser that is able to parse all the transaction types for each protocol.</li>
            <li>Write test for the generic parser.</li>
            <li>Add ability to add rules for each protocol/transaction type through ui.</li>
            <li>Write unit and e2e test for adding rules through ui </li>
            <li>Protect ui to allow only authenticated users to add protocols/transaction types.</li>
        </ol>
    * Deliverables:
        * Generic Classifier & Parser
        * Add ui for managing protocols & transaction types
        * Minimal Support: Anchor, Mirror, Terraswap, Nexus, Valkyre, Mars, Astroport
* ### **Add support for tax software(Max: 3)**
    * Est. Duration: 5 days
    * Funding: $3,200
    * Deliverables:
        * Users will be able to filter the transaction by date, transaction type.
        * Users will be able to export the data to three supported third-pary apps based on their filter.
* ### **Add support for REST and GraphQL**
    * Est. Duration: 5 days
    * Funding: $3,200
    * Deliverable:
        * This will allow interacting with the application for third-party apps and query based on
            * Wallet address
            * Transaction type
            * Transaction date

