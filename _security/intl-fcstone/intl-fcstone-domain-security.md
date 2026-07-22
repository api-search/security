---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: intl-fcstone.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stonex.com
  spf: true
hosts:
- host: www.intl-fcstone.com
  https: false
- cert_expires: Aug 16 23:11:03 2026 GMT
  host: www.stonex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Intl Fcstone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for INTL FCStone, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: INTL FCStone
provider_slug: intl-fcstone
slug: intl-fcstone-domain-security
source_filename: intl-fcstone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.intl-fcstone.com\n  https: false\n- host: www.stonex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 23:11:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: intl-fcstone.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: stonex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/intl-fcstone/refs/heads/main/security/intl-fcstone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Commodities
- Foreign Exchange
- Risk Management
- Trading
- Market Intelligence
- Fortune 100
---
