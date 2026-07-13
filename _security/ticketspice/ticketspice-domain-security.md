---
api_specs:
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Forms and Inventory API
  slug: ticketspice-forms-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Orders and Registrants API
  slug: ticketspice-orders-registrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Tickets API
  slug: ticketspice-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Transactions and Customers API
  slug: ticketspice-transactions-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Coupons API
  slug: ticketspice-coupons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
- filename: ticketspice-openapi.yml
  format: yaml
  label: TicketSpice Webhooks API
  slug: ticketspice-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/openapi/ticketspice-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@webconnex.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ticketspice.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: webconnex.io
  spf: true
hosts:
- cert_expires: Oct  1 08:06:36 2026 GMT
  host: www.ticketspice.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: docs.webconnex.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 13 01:24:20 2026 GMT
  host: api.webconnex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ticketspice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TicketSpice, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TicketSpice
provider_slug: ticketspice
slug: ticketspice-domain-security
source_filename: ticketspice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ticketspice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 08:06:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.webconnex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: false\n- host: api.webconnex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 01:24:20 2026 GMT\n  hsts: null\ndomains:\n- domain: ticketspice.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@webconnex.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: webconnex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ticketspice/refs/heads/main/security/ticketspice-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Ticketing
- Ticketing
- Events
- Registration
- Payments
- Webconnex
---
