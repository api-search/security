---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:security@betterment.com"
  - 0 issue "amazontrust.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: betterment.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: plaid.com
  spf: true
hosts:
- cert_expires: Sep 20 05:47:31 2026 GMT
  host: www.betterment.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- host: api.betterment.com
  https: false
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: plaid.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betterment Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betterment, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Betterment
provider_slug: betterment
slug: betterment-domain-security
source_filename: betterment-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betterment.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 05:47:31 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: api.betterment.com\n  https: false\n- host: plaid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: betterment.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@betterment.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: plaid.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterment/refs/heads/main/security/betterment-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Robo-Advisor
- Automated Investing
- Financial Planning
- Tax-Loss Harvesting
- Retirement Planning
- Portfolio Management
- 401k
- Fintech
- Wealth Management
- Investment Rebalancing
- Open Banking
---
