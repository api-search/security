---
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:security@monzo.com"
  - 0 issue "amazon.com"
  - 0 issue "buypass.com"
  - 0 issue "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: monzo.com
  spf: true
hosts:
- cert_expires: Feb 27 23:59:59 2027 GMT
  host: monzo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:25:15 2026 GMT
  host: docs.monzo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 03:25:15 2026 GMT
  host: api.monzo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Monzo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monzo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Monzo
provider_slug: monzo
slug: monzo-domain-security
source_filename: monzo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.monzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:25:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.monzo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 03:25:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: monzo.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:security@monzo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"buypass.com\"\n  - 0 issue \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monzo/refs/heads/main/security/monzo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Banking
- Fintech
- Financial Services
- Payments
- Open Banking
- Accounts
- Transactions
- OAuth
---
