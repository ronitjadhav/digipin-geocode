# digipin

`digipin` is an npm package that allows you to convert between latitude/longitude coordinates and Digital Postal Index Numbers (DIGIPINs). This system is part of an initiative by the Department of Posts in India to create a standardized, geo-coded addressing system. For more details, please visit the [India Post DIGIPIN](https://www.indiapost.gov.in/vas/Pages/digipin.aspx).

## Features

- Convert latitude and longitude to DIGIPIN
- Convert DIGIPIN to latitude and longitude

## Installation

To install the package, use npm or yarn:

```bash
npm install digipin
```

## Usage

### Importing the Functions

You can import the functions either as named imports or as a default import.

#### Named Imports

```typescript
import { getDIGIPINFromLatLon, getLatLonFromDIGIPIN } from 'digipin';

const digipin = getDIGIPINFromLatLon(12.34, 56.78);
console.log(digipin); // Outputs the corresponding DIGIPIN

const coordinates = getLatLonFromDIGIPIN('G4J-9K4-7L');
console.log(coordinates); // Outputs the corresponding latitude and longitude
```


#### Default Import

```typescript
import digipin from 'digipin';

const digipinCode = digipin.getDIGIPINFromLatLon(12.34, 56.78);
console.log(digipinCode); // Outputs the corresponding DIGIPIN

const coordinates = digipin.getLatLonFromDIGIPIN('G4J-9K4-7L');
console.log(coordinates); // Outputs the corresponding latitude and longitude
```

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your changes. For major changes, please open an issue to discuss what you would like to change.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.