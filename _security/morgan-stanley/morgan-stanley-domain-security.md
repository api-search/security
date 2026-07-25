---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: morganstanley.com
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:domains@etrade.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: etrade.com
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: www.morganstanley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 21 23:59:59 2027 GMT
  host: developer.morganstanley.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: developer.etrade.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Morgan Stanley Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morgan Stanley, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Morgan Stanley
provider_slug: morgan-stanley
slug: morgan-stanley-domain-security
source_filename: morgan-stanley-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.morganstanley.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.morganstanley.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.etrade.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: morganstanley.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: etrade.com\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:domains@etrade.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/morgan-stanley/refs/heads/main/security/morgan-stanley-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Financial
- Investment Banking
- Wealth Management
- Brokerage
- Market Data
- Trading
- Fortune 100
- United States
---
