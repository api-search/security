---
api_specs:
- filename: kard-api-reference-openapi.yaml
  format: yaml
  label: Kard Rewards API
  slug: kard-rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/openapi/kard-api-reference-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: getkard.com
  spf: true
hosts:
- cert_expires: Aug 24 20:29:31 2026 GMT
  host: getkard.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kard
provider_slug: kard
slug: kard-domain-security
source_filename: kard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getkard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 20:29:31 2026 GMT\n  hsts: null\ndomains:\n- domain: getkard.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kard/refs/heads/main/security/kard-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Rewards
- Card-Linked Offers
- Loyalty
- Fintech
- Commerce Media
- Advertising
- Transactions
- Cashback
- Webhooks
---
