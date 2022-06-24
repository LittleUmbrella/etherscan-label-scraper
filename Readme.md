# etherscan-label-scraper
[![Build Status](https://app.travis-ci.com/Beasta/etherscan-label-scraper.svg?branch=master)](https://app.travis-ci.com/Beasta/etherscan-label-scraper)

Retrieve the etherscan label for a specific ethereum address. No API keys required! Its unfortunate that Etherscan won't provide API access to this information.
## Installation

```
npm install etherscan-label-scraper
```

## Usage
```js
async function f() {
    let addressScraper = await import('etherscan-label-scraper');
    addressScraper = addressScraper.default();
    const address = '0x829bd824b016326a401d083b33d092293333a830';
    console.log(await addressScraper.requestEtherscan(address));
    // { fullLabel: 'F2Pool Old' }
}
f();
```
## Running the tests

```
npm test
```

## License
MIT

