---
description: ''
domains:
- caa:
  - 0 iodef "mailto:hostmaster@visa.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: authorize.net
  spf: true
hosts:
- cert_expires: Oct 18 20:44:37 2026 GMT
  host: www.authorize.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 02:27:05 2026 GMT
  host: developer.authorize.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.authorize.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Authorize Net Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authorize.net, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Authorize.net
provider_slug: authorize-net
slug: authorize-net-domain-security
source_filename: authorize-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.authorize.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 20:44:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.authorize.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 02:27:05 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.authorize.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: authorize.net\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:hostmaster@visa.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authorize-net/refs/heads/main/security/authorize-net-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Accept.js
- Credit Cards
- eChecks
- Fraud Detection
- Payment Gateway
- Payments
- Recurring Billing
- Transactions
---
