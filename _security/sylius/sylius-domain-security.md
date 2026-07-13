---
api_specs:
- filename: docs.json
  format: json
  label: Sylius REST API
  slug: sylius-api
  spec_type: OpenAPI
  url: https://your-sylius-instance.com/api/v2/docs.json
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sylius.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: your-sylius-instance.com
  spf: false
hosts:
- cert_expires: Aug 22 16:39:47 2026 GMT
  host: sylius.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 01:13:14 2026 GMT
  host: docs.sylius.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-sylius-instance.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sylius Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sylius, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sylius
provider_slug: sylius
slug: sylius-domain-security
source_filename: sylius-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sylius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 16:39:47 2026 GMT\n  hsts: false\n- host: docs.sylius.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 01:13:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-sylius-instance.com\n  https: false\ndomains:\n- domain: sylius.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: your-sylius-instance.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sylius/refs/heads/main/security/sylius-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eCommerce
- Open Source
- Headless Commerce
- REST API
- Symfony
- PHP
- Products
- Orders
- Payments
- Shipments
- Customers
---
