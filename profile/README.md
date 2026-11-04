# Beziworld: Laravel packages for Polish business integrations

Open-source Laravel packages for payments, invoicing and KSeF, couriers, marketplaces, SMS, hotels, hosting and
Polish public registers. Created and maintained by **Kamil Ćwiertnia**, [beziworld.eu](https://beziworld.eu).

Every package supports PHP 8.3+ and Laravel 12-13, is tested with Pest and analysed with PHPStan level 8, ships a
facade, publishable config and documentation in English and Polish, and installs with Composer:

```bash
composer require beziworld/laravel-<name>
```

## Payments

| Package | What it does |
|---|---|
| [laravel-przelewy24](https://github.com/Beziworld/laravel-przelewy24) | Przelewy24: transactions, verification, refunds, signed notifications |
| [laravel-tpay](https://github.com/Beziworld/laravel-tpay) | Tpay OpenAPI: transactions, BLIK, refunds, JWS-signed notifications |
| [laravel-payu](https://github.com/Beziworld/laravel-payu) | PayU: orders, capture, refunds, payment methods, signed notifications |
| [laravel-paynow](https://github.com/Beziworld/laravel-paynow) | Paynow (mBank): payments, BLIK, refunds, HMAC-signed notifications |
| [laravel-autopay](https://github.com/Beziworld/laravel-autopay) | Autopay (Blue Media): transactions, ITN notifications, gateway list, refunds |
| [laravel-imoje](https://github.com/Beziworld/laravel-imoje) | imoje (ING): payment links, transactions, BLIK, refunds, signed notifications |

## Invoicing and KSeF

| Package | What it does |
|---|---|
| [laravel-ksef](https://github.com/Beziworld/laravel-ksef) | KSeF 2.0: token authentication, encrypted sessions, FA(3) builder validated against the official XSD, UPO, QR links |
| [laravel-fakturownia](https://github.com/Beziworld/laravel-fakturownia) | Fakturownia: invoices, PDF, e-mail, payments, clients, products, KSeF submission |
| [laravel-infakt](https://github.com/Beziworld/laravel-infakt) | inFakt API v3: asynchronous invoice creation, PDF, payments, e-mail, clients |
| [laravel-wfirma](https://github.com/Beziworld/laravel-wfirma) | wFirma: invoices, contractors, goods, PDF, e-mail |
| [laravel-ifirma](https://github.com/Beziworld/laravel-ifirma) | iFirma: HMAC-signed invoices, payments, KSeF submission |

## Couriers and shipping

| Package | What it does |
|---|---|
| [laravel-inpost](https://github.com/Beziworld/laravel-inpost) | InPost ShipX: shipments, parcel lockers, labels, tracking, status webhooks |
| [laravel-dpd](https://github.com/Beziworld/laravel-dpd) | DPD Polska: shipments, labels, protocols, pickups, tracking, DPD Pickup points |
| [laravel-dhl-parcel](https://github.com/Beziworld/laravel-dhl-parcel) | DHL Parcel Polska (DHL24 WebAPI2): shipments, labels, courier booking, tracking |
| [laravel-orlen-paczka](https://github.com/Beziworld/laravel-orlen-paczka) | ORLEN Paczka: parcels, labels, tracking, all pickup points |
| [laravel-gls](https://github.com/Beziworld/laravel-gls) | GLS Poland ADE-Plus: consignments, labels, pickup confirmations, ParcelShop, services, tracking |
| [laravel-furgonetka](https://github.com/Beziworld/laravel-furgonetka) | Furgonetka.pl: OAuth2, prices, packages, order commands, labels, points |
| [laravel-apaczka](https://github.com/Beziworld/laravel-apaczka) | Apaczka.pl: valuation, orders, waybills, pickups, signed tracking webhooks |

## Marketplaces and e-commerce

| Package | What it does |
|---|---|
| [laravel-allegro](https://github.com/Beziworld/laravel-allegro) | Allegro REST API: OAuth2 (PKCE, device flow), multi-seller, order and offer event polling, Wysyłam z Allegro |
| [laravel-baselinker](https://github.com/Beziworld/laravel-baselinker) | BaseLinker: all 211 API methods, multiple accounts, journal polling, rate limiting |

## SMS and messaging

| Package | What it does |
|---|---|
| [laravel-smsapi](https://github.com/Beziworld/laravel-smsapi) | SMSAPI: SMS sending, notification channel, delivery reports |
| [laravel-serwersms](https://github.com/Beziworld/laravel-serwersms) | SerwerSMS.pl: SMS, MMS, voice, HLR, notification channel |
| [laravel-smsplanet](https://github.com/Beziworld/laravel-smsplanet) | SMSPlanet.pl: SMS, MMS, signed delivery webhooks, notification channel |
| [laravel-twilio](https://github.com/Beziworld/laravel-twilio) | Twilio: SMS, WhatsApp, Verify, Lookup, signed webhooks, notification channel |

## Hotels

| Package | What it does |
|---|---|
| [laravel-previo](https://github.com/Beziworld/laravel-previo) | Previo PMS: XML, REST, POS and EQC APIs, many accounts and hotels, reservations, guests, billing |

## Polish registers, data and utilities

| Package | What it does |
|---|---|
| [laravel-company-data](https://github.com/Beziworld/laravel-company-data) | GUS REGON (BIR), VAT white list with bank account checks, EU VIES |
| [laravel-krs](https://github.com/Beziworld/laravel-krs) | KRS open API: company extracts, board and representation, shareholders, status flags, daily change bulletin watcher |
| [laravel-ceidg](https://github.com/Beziworld/laravel-ceidg) | CEIDG API v3: sole proprietorships by NIP or REGON, register search, validation rule, status watcher |
| [laravel-uldk](https://github.com/Beziworld/laravel-uldk) | GUGiK ULDK: cadastral parcels and administrative units by id or coordinates, WKT/GeoJSON |
| [laravel-nbp](https://github.com/Beziworld/laravel-nbp) | NBP exchange rates and gold prices, VAT invoice rate rule, currency conversion |
| [laravel-polish-validation](https://github.com/Beziworld/laravel-polish-validation) | Validation rules: PESEL, NIP, REGON, KRS, IBAN/NRB, ID card, postal code, phone |
| [laravel-polish-calendar](https://github.com/Beziworld/laravel-polish-calendar) | Polish public holidays and business day calculations, Carbon macros, rules |

## Hosting and DNS

| Package | What it does |
|---|---|
| [laravel-directadmin](https://github.com/Beziworld/laravel-directadmin) | DirectAdmin: users, domains, e-mail, databases, DNS, SSL, cron, backups |
| [laravel-cpanel](https://github.com/Beziworld/laravel-cpanel) | cPanel UAPI and WHM: accounts, packages, SSO, domains, DNS, e-mail, MySQL, SSL, FTP, cron, backups |
| [laravel-plesk](https://github.com/Beziworld/laravel-plesk) | Plesk REST and XML API: customers, subscriptions, DNS, databases, mail, Let's Encrypt, CLI gate |
| [laravel-cloudflare](https://github.com/Beziworld/laravel-cloudflare) | Cloudflare API v4: zones, DNS, cache purge, SSL/TLS, WAF, Turnstile rule, trusted proxies middleware |

## Need an integration?

Custom integrations with Polish and European services, KSeF, payments, couriers and marketplaces:
[beziworld.eu](https://beziworld.eu) · [biuro@beziworld.eu](mailto:biuro@beziworld.eu)
