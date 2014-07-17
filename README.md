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
//   secure: true }
```

## Supported services

Service names are case insensitive

  * **'AOL'**
  * **'DynectEmail'**
  * **'FastMail'**
  * **'Gmail'**
  * **'Godaddy'**
  * **'GodaddyAsia'**
  * **'GodaddyEurope'**
  * **'hot.ee'**
  * **'Hotmail'**
  * **'iCloud'**
  * **'mail.ee'**
  * **'Mail.ru'**
  * **'Mailgun'**
  * **'Mailjet'**
  * **'Mandrill'**
  * **'Postmark'**
  * **'QQ'**
  * **'QQex'**
  * **'SendCloud'**
  * **'SendGrid'**
  * **'SES'**
  * **'Yahoo'**
  * **'Yandex'**
  * **'Zoho'**

### Example usage with Nodemailer

```javascript
var transporter = nodemailer.createTransport({
     service: 'postmark' // <- resolved as 'Postmark' from the wellknown info
     auth: {...}
});
```

## License

**MIT**