# deck-of-cards-postman-tests

## Summary

A Postman collection for the [Deck of Cards API](https://deckofcardsapi.com/) that includes tests.

## Prerequisites

- Postman (last tested with version 8.11.1)
- Node.js (last tested with version LTS 14.17.5)
- Newman (last tested with version 5.2.4)

## How to run tests

### Postman GUI

1. Clone this repository (`git clone https://github.com/Jmcosel/deck-of-cards-postman-tests.git`)
2. Open Postman and [import deck_of_cards_api.postman_collection.json](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/)
3. Use the [Collection Runner](https://learning.postman.com/docs/running-collections/intro-to-collection-runs/) to run the test suite. Make sure to specify the `deck_data.csv` file for data variables.

### Newman CLI

1. Clone this repository (`git clone https://github.com/Jmcosel/deck-of-cards-postman-tests.git`)
2. Simply run the following command: `newman run deck_of_cards_api.postman_collection.json -d deck_data.csv`
