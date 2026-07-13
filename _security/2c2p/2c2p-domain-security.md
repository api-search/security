---
api_specs:
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Token API
  slug: 2c2p-payment-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Do Payment API
  slug: 2c2p-do-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Option API
  slug: 2c2p-payment-option-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Inquiry API
  slug: 2c2p-payment-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Payment Maintenance API
  slug: 2c2p-payment-maintenance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Card Token & Recurring API
  slug: 2c2p-card-token-recurring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
- filename: 2c2p-openapi.yml
  format: yaml
  label: 2C2P Exchange Rate API
  slug: 2c2p-exchange-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/openapi/2c2p-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issue "geotrust.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "rapidssl.com"
  - 0 issue "sectigo.com"
  - 0 issue "securetrust.com"
  - 0 issue "symantec.com"
  - 0 issue "thaidigitalid.com"
  - 0 issue "thawte.com"
  - 0 issue "visa.com"
  - 0 issue "amazon.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_pct: 25
  dmarc_policy: quarantine
  dnssec: false
  domain: 2c2p.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:mail.zendesk.com include:sendgrid.net include:amazonses.com include:44900109.spf01.hubspotemail.net ~all
hosts:
- cert_expires: Oct 18 03:00:23 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: 2c2p.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 03:00:23 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: www.2c2p.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  http_status: 301
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 13:01:55 2026 GMT
  cert_issuer: Let's Encrypt (YE2)
  host: developer.2c2p.com
  hsts: true
  hsts_include_subdomains: false
  hsts_max_age: 31536000
  http_status: 302
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 18 03:00:23 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: pgw.2c2p.com
  hsts: false
  http_status: 403
  https: true
  note: Production PGW API host. Returns 403 to unauthenticated GET; expects signed JWT POST to /payment/4.3/* endpoints.
  tls_version: TLSv1.2
- cert_expires: Oct 18 03:00:23 2026 GMT
  cert_issuer: GlobalSign RSA OV SSL CA 2018
  host: sandbox-pgw.2c2p.com
  hsts: false
  http_status: 403
  https: true
  note: Sandbox PGW API host. Returns 403 to unauthenticated GET; expects signed JWT POST.
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: 2C2P Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 2C2P, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 2C2P
provider_slug: 2c2p
slug: 2c2p-domain-security
source_filename: 2c2p-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + PGW API hosts\nhosts:\n- host: 2c2p.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Oct 18 03:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 200\n- host: www.2c2p.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Oct 18 03:00:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  http_status: 301\n- host: developer.2c2p.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Let's Encrypt (YE2)\n  cert_expires: Sep 23 13:01:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: false\n  http_status: 302\n- host: pgw.2c2p.com\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires:\
  \ Oct 18 03:00:23 2026 GMT\n  hsts: false\n  http_status: 403\n  note: Production PGW API host. Returns 403 to unauthenticated GET; expects signed JWT POST to /payment/4.3/* endpoints.\n- host: sandbox-pgw.2c2p.com\n  https: true\n  tls_version: TLSv1.2\n  cert_issuer: GlobalSign RSA OV SSL CA 2018\n  cert_expires: Oct 18 03:00:23 2026 GMT\n  hsts: false\n  http_status: 403\n  note: Sandbox PGW API host. Returns 403 to unauthenticated GET; expects signed JWT POST.\ndomains:\n- domain: 2c2p.com\n  dnssec: false\n  caa:\n  - '0 issue \"digicert.com\"'\n  - '0 issue \"entrust.net\"'\n  - '0 issue \"geotrust.com\"'\n  - '0 issue \"globalsign.com\"'\n  - '0 issue \"letsencrypt.org\"'\n  - '0 issue \"rapidssl.com\"'\n  - '0 issue \"sectigo.com\"'\n  - '0 issue \"securetrust.com\"'\n  - '0 issue \"symantec.com\"'\n  - '0 issue \"thaidigitalid.com\"'\n  - '0 issue \"thawte.com\"'\n  - '0 issue \"visa.com\"'\n  - '0 issue \"amazon.com\"'\n  - '0 issue \"comodoca.com\"'\n  spf: true\n  spf_record:\
  \ v=spf1 include:_spf.google.com include:mail.zendesk.com include:sendgrid.net include:amazonses.com include:44900109.spf01.hubspotemail.net ~all\n  dmarc: true\n  dmarc_policy: quarantine\n  dmarc_pct: 25\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/2c2p/refs/heads/main/security/2c2p-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Payments
- Payment Gateway
- Southeast Asia
- Singapore
- Thailand
- Cards
- E-Wallet
- Payment Token
- Cross-Border
- Fintech
---
