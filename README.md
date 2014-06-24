# Nodemailer Well-Known Services

Returns SMTP configuration for well-known services

## Usage

Install with npm

    npm install nodemailer-wellknown

Require in your script

```javascript
var wellknown = require('nodemailer-wellknown');
```

Resolve SMTP settings

```javascript
var config = wellknown('Gmail');
// { host: 'smtp.gmail.com',
//   port: 465,
//   secureConnection: true }
```

## License

**MIT**