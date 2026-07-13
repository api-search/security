---
api_specs:
- filename: llms.txt
  format: yaml
  label: Tango RaaS API
  slug: tango-raas-api
  spec_type: OpenAPI
  url: https://developers.tangocard.com/llms.txt
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tangocard.com
  spf: true
hosts:
- cert_expires: Aug 24 15:43:14 2026 GMT
  host: www.tangocard.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 18:11:01 2026 GMT
  host: developers.tangocard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.tangocard.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tango Card Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tango Card, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tango Card
provider_slug: tango-card
slug: tango-card-domain-security
source_filename: tango-card-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tangocard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 15:43:14 2026 GMT\n  hsts: false\n- host: developers.tangocard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 18:11:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tangocard.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tangocard.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tango-card/refs/heads/main/security/tango-card-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Gift Cards
- Rewards
- Incentives
- Digital Rewards
- Prepaid Cards
- Payments
---
