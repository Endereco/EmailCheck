# EmailCheck

Checks the entered email for valid syntax and for the possibility to deliver.

## Installation

In order to pull the latest version:

### npm (preferred)

```
npm i @endereco/emailcheck
```

### github

```
git clone https://github.com/Endereco/EmailCheck.git
```

Then include EmailCheck.js in `<header>` or before config.

## Configuration

In order to use email check you must specify the field for email.

Here is an example configuration:

```
new EmailCheck({
    'inputSelector': 'input[name="register[personal][email]"]',
    'endpoint': 'https://example-domain.com/endpoint',
    'apiKey': '041c3c302746cf37722560a7a285690738a7db4e55b7aaf26a545ffabd318a83'
});
```

## Dependencies

EmailCheck relies on StatusIndicator to mark fields green on correct input.

EmailCheck also relies on Accounting to generate the tid and track transactions.
