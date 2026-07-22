---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moment.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: moment-api.com
  spf: false
hosts:
- cert_expires: Oct  4 09:37:06 2026 GMT
  host: moment.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 03:12:09 2026 GMT
  host: docs.moment.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: moment-api.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''moment-api.'
kind: domain-security
layout: security
method: probed
name: Moment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Moment, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Moment
provider_slug: moment
slug: moment-domain-security
source_filename: moment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 09:37:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.moment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 03:12:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: moment-api.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''moment-api.'\n  hsts: null\ndomains:\n- domain: moment.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moment-api.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moment/refs/heads/main/security/moment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fixed Income
- Bonds
- Trading
- Market Data
- Reference Data
- Investment Management
- Wealth Management
- Brokerage
- Financial Services
- Fintech
---
