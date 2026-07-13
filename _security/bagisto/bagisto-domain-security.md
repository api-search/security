---
api_specs:
- filename: rest-api.html
  format: yaml
  label: Bagisto REST API
  slug: bagisto-rest-api
  spec_type: OpenAPI
  url: https://devdocs.bagisto.com/api/rest-api.html
description: ''
domains:
- caa:
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bagisto.com
  spf: true
hosts:
- cert_expires: Aug 29 16:29:50 2026 GMT
  host: bagisto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 16:29:50 2026 GMT
  host: api-docs.bagisto.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 09:39:48 2026 GMT
  host: devdocs.bagisto.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bagisto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bagisto, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Bagisto
provider_slug: bagisto
slug: bagisto-domain-security
source_filename: bagisto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bagisto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:29:50 2026 GMT\n  hsts: false\n- host: api-docs.bagisto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 16:29:50 2026 GMT\n  hsts: false\n- host: devdocs.bagisto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 09:39:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: bagisto.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bagisto/refs/heads/main/security/bagisto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Laravel
- Open Source
- Products
- Orders
- Customers
- Inventory
- Multi-Channel
- Headless Commerce
---
