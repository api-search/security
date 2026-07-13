---
api_specs:
- filename: reloadly-gift-cards-openapi.yml
  format: yaml
  label: Reloadly Gift Cards API
  slug: gift-cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-gift-cards-openapi.yml
- filename: reloadly-airtime-openapi.yml
  format: yaml
  label: Reloadly Airtime API
  slug: airtime
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/openapi/reloadly-airtime-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issue "amazon.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: reloadly.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: www.reloadly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: giftcards.reloadly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: topups.reloadly.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Reloadly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reloadly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Reloadly
provider_slug: reloadly
slug: reloadly-domain-security
source_filename: reloadly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.reloadly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: false\n- host: giftcards.reloadly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\n- host: topups.reloadly.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: reloadly.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reloadly/refs/heads/main/security/reloadly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Gift Cards
- Payments
- Airtime
- Mobile Top-Up
- Rewards
- Incentives
---
