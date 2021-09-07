<p align="center">
  <a><img src="./images/qualear.png" width=180 height="180"></a>
  <h1 align="center">Qualear - Reconnaissance Apparatus</h1>
  <p align="center">
    <a href="https://goreportcard.com/report/github.com/maraudery/qualear"><img src="https://goreportcard.com/badge/github.com/maraudery/qualear" alt="Go Report Card"></a>
    <a><img src="https://img.shields.io/badge/tests-7&#47;8-orange.svg" alt="s"></a>
    <a><img src="https://img.shields.io/badge/version-0.6.0-blue.svg" alt="s"></a>
    <a href="https://pkg.go.dev/github.com/maraudery/qualear"><img src="https://pkg.go.dev/badge/github.com/maraudery/qualear.svg" alt="Go Report Card"></a>
    <a href="https://inventory.raw.pm/"><img src="https://inventory.raw.pm/img/badges/Rawsec-inventoried-FF5050_flat.svg" alt="Rawsec&#39;s CyberSecurity Inventory"></a><br>
    Centralize and expedite the reconnaissance process.
</a>
  </p><br>
</p>

## Table of Contents

- [Information](#information)
  - [About](#about)
  - [Disclaimer](#disclaimer)
  - [Preview](#preview)
  - [Installation](#installation)
  - [Usage](#usage)
  - [API](#api)
  - [Implementation](#implementation)
  - [Testing](#testing)
  - [Attributions](#attributions)
- [Package Types](#package-types) *a-z*
  - [Court Cases](#court-cases)
  - [Discord](#discord)
  - [IP Address](#ip-address)
  - [Multi-Use](#multi-use)
  - [Username](#username)
  - [Vehicle](#vehicle)



## Information

### About

Qualear is a reconnaissance apparatus that aims to centralize all of the tools necessary to carry out an open-source intelligence investigation. Although investigations will still require human interaction to connect the dots, the interface can be tailored to an individual’s needs to expedite the process of due diligence. Some packages do require an authentication key and others do not. See the [Package Types](#package-types) tables for more information. Qualear can be integrated within your application OR it can be used directly from the [terminal/web browser.](#preview)

### Disclaimer

It is the end user's responsibility to obey all applicable local, state, and federal laws. Developers assume no liability and are not responsible for any misuse or damage caused by this program. By using Qualear, you agree to the previous statements.

### Preview

<a><img src="./images/cliprev.png" width=660 height="360"></a>
<a><img src="./images/guiprev.png" width=660 height="360"></a>

### Installation

 - Fetch the repository via 'git clone': `git clone https://github.com/maraudery/qualear.git`

### Usage

1. Navigate into the root directory of Qualear.
2. In your preferred terminal, enter and run: `go run main.go`
3. After running the aforementioned command, all dependencies will be installed and usage help will be printed to the console.

### API

1. Navigate into the `api` directory of Qualear.
2. In your preferred terminal, enter and run: `go run server.go`
3. When prompted, allow the application to communicate on your network.
4. Navigate to `http://localhost:6174/`

### Implementation

Instructions/Documentation are provided for each and every package, all you have to do is find what you need in the [Package Types](#package-types) section.

### Testing

Qualear is currently passing all tests; however, I have provided instructions for properly running the tests if you would like to do so.

1. In the root directory of Qualear, create a file named `keyconfig.json`
2. In `keyconfig.json`, paste the following text:
``` json
{
    "melissaKeyCred": "Paste Melissa Key with Credits Here",
    "hibpKey": "Paste Have I Been Pwned Key Here",
    "dataGovKey": "Paste Data.gov Key Here"
}
```
3. Paste in your API keys. The test will fail without a valid API key.
4. In your preferred terminal, enter and run `go test ./...`

### Attributions

[Logo](./images/qualear.png) created with and licensed by [LogoMakr CC License.](https://my.logomakr.com/cc-license/)

[Card](./images/card.jpg) created with [Canva.](https://www.canva.com/)

## Package-Types

### Court Cases

| Package                                                                                    | Description                                  |   Auth   |
| :----------------------------------------------------------------------------------------: | -------------------------------------------- | :------: |
| [Case Law](https://github.com/maraudery/qualear/tree/main/pkg/noauth/caselaw)           | Court Case Search                            |  `none`  |

### IP Address

| Package                                                                                    | Description                                  |   Auth   |
| :----------------------------------------------------------------------------------------: | -------------------------------------------- | :------: |
| [IPV4 Address Lookup](https://github.com/maraudery/qualear/tree/main/pkg/noauth/ip)     | IPV4 Address Lookup                          |  `none`  |

### Multi-Use

| Package                                                                                    | Description                                  |   Auth   |
| :----------------------------------------------------------------------------------------: | -------------------------------------------- | :------: |
| [Have I Been Pwned](https://github.com/maraudery/qualear/tree/main/pkg/authpaid/hibp)   | Email and Password Vulnerability - (Breaches)|  `paid`  |
| [Melissa](https://github.com/maraudery/qualear/tree/main/pkg/authfree/melissa)          | Lookups - Email, Phone Number, IP Address    |  `free`  |


### Username

| Package                                                                                    | Description                                  |   Auth   |
| :----------------------------------------------------------------------------------------: | -------------------------------------------- | :------: |
| [Username Lookup](https://github.com/maraudery/qualear/tree/main/pkg/noauth/userlookup) | Username Lookup - (Comparable to Sherlock)   |  `none`  |

### Vehicle

| Package                                                                                    | Description                                  |   Auth   |
| :----------------------------------------------------------------------------------------: | -------------------------------------------- | :------: |
| [VIN Lookup](https://github.com/maraudery/qualear/tree/main/pkg/noauth/vin)             | Vehicle Identification Number Lookup         |  `none`  |
