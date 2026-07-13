---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: shiphero.com
  spf: true
hosts:
- cert_expires: Sep  5 23:58:56 2026 GMT
  host: shiphero.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 18:27:19 2026 GMT
  host: developer.shiphero.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: public-api.shiphero.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Shiphero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ShipHero, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ShipHero
provider_slug: shiphero
slug: shiphero-domain-security
source_filename: shiphero-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: shiphero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:58:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.shiphero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 18:27:19 2026 GMT\n  hsts: false\n- host: public-api.shiphero.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: shiphero.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shiphero/refs/heads/main/security/shiphero-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Warehouse Management
- Fulfillment
- eCommerce
- GraphQL
- Inventory
- Orders
- Shipments
- 3PL
- Logistics
---
