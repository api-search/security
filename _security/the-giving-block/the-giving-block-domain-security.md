---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: thegivingblock.com
  spf: true
hosts:
- cert_expires: Sep 22 14:02:29 2026 GMT
  host: thegivingblock.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Giving Block Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Giving Block, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: The Giving Block
provider_slug: the-giving-block
slug: the-giving-block-domain-security
source_filename: the-giving-block-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thegivingblock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 14:02:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: thegivingblock.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-giving-block/refs/heads/main/security/the-giving-block-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Donations
- Fundraising
- Nonprofit
- Payments
- Cryptocurrency
- Stock Donations
- Webhooks
- Widgets
---
