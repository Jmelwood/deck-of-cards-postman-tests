# Deck of Cards Postman API Tests

## Summary

A Postman collection for the [Deck of Cards API](https://deckofcardsapi.com/) that includes tests.
These are mostly happy path workflow tests with a couple of common scenarios attached via the `data_tests.csv` file. Postman is not a great place to do boundary/unit testing.

## Prerequisites

- Postman (last tested with version 11.6.2)
- Node.js (last tested with version LTS 20.15.1)
- Newman (last tested with version 6.1.3) - install via NPM

## How to run tests

### Postman GUI

1. Clone this repository (`git clone https://github.com/Jmelwood/deck-of-cards-postman-tests.git`)
2. Open Postman and [import deck_of_cards_api.postman_collection.json](https://learning.postman.com/docs/getting-started/importing-and-exporting-data/)
3. Use the [Collection Runner](https://learning.postman.com/docs/running-collections/intro-to-collection-runs/) to run the test suite. Make sure to specify the `deck_data.csv` file for data variables.

### Newman CLI

1. Clone this repository (`git clone https://github.com/Jmelwood/deck-of-cards-postman-tests.git`)
2. Simply run the following command: `newman postman/run deck_of_cards_api.postman_collection.json -d deck_data.csv`
