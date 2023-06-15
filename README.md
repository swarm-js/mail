![Version](https://img.shields.io/npm/v/@swarmjs/mail) ![Downloads](https://img.shields.io/npm/dm/@swarmjs/mail) ![License](https://img.shields.io/github/license/swarm-js/mail) ![Build](https://img.shields.io/github/actions/workflow/status/swarm-js/mail/build.yml?branch=main)
<br/>

<p align="center">
  <a href="https://github.com/swarm-js/mail">
    <img src="images/logo.png" alt="Logo" width="120" height="120">
  </a>

  <h3 align="center">@swarmjs/mail</h3>

  <p align="center">
    HTML email notification generator.
    <br/>
    <br/>
  </p>
</p>

## Table Of Contents

- [About the Project](#about-the-project)
- [Built With](#built-with)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Roadmap](#roadmap)
- [Contributing](#contributing)
- [License](#license)
- [Mailors](#mailors)
- [Acknowledgements](#acknowledgements)

## About The Project

This package aims to help developers quickly create simple and clean HTML notification emails.

## Built With

- TypeScript@4

## Getting Started

### Installation

```sh
yarn add @swarmjs/mail
```

or

```sh
npm install --save @swarmjs/mail
```

## Usage

```ts
import { Mail } from '@swarmjs/mail'
const html = Mail.create('Email preview message')
  .header({
    logo: 'https://www.example.com/image.png'n
    title: 'Login with a magic link'
  })
  .text(
    `Here some text`
  )
  .button(
    'Button text',
    `http://example.com/url`
  )
  .alert({
     title: 'Alert title',
      description: 'Alert description',
      windowTitle: 'ALERT',
      buttonText: 'More details',
      url: 'https://www.example.com',
  })
  .warning({
     title: 'Alert title',
      description: 'Alert description',
      windowTitle: 'ALERT',
      buttonText: 'More details',
      url: 'https://www.example.com',
  })
  .info({
     title: 'Alert title',
      description: 'Alert description',
      windowTitle: 'ALERT',
      buttonText: 'More details',
      url: 'https://www.example.com',
  })
  .success({
     title: 'Alert title',
      description: 'Alert description',
      windowTitle: 'ALERT',
      buttonText: 'More details',
      url: 'https://www.example.com',
  })
  .spacer(20) // add 20px space
  .end()
```

## Roadmap

See the [open issues](https://github.com/swarm-js/mail/issues) for a list of proposed features (and known issues).

## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

- If you have suggestions for adding or removing projects, feel free to [open an issue](https://github.com/swarm-js/mail/issues/new) to discuss it, or directly create a pull request after you edit the _README.md_ file with necessary changes.
- Please make sure you check your spelling and grammar.
- Create individual PR for each suggestion.
- Please also read through the [Code Of Conduct](https://github.com/swarm-js/mail/blob/main/CODE_OF_CONDUCT.md) before posting your first idea as well.

### Creating A Pull Request

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See [LICENSE](https://github.com/swarm-js/mail/blob/main/LICENSE.md) for more information.

## Mailors

- [Guillaume Gagnaire](https://github.com/guillaume-gagnaire)
