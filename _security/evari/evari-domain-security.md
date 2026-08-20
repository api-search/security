---
api_specs:
- filename: evari-quotes-api-openapi.yml
  format: yaml
  label: Evari Quotes API
  slug: evari-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/evari/refs/heads/main/openapi/evari-quotes-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: evari.tech
  spf: true
hosts:
- cert_expires: Oct 10 02:22:48 2026 GMT
  host: evari.tech
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Evari
provider_slug: evari
slug: evari-domain-security
source_filename: evari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evari.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 02:22:48 2026 GMT\n  hsts: null\ndomains:\n- domain: evari.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evari/refs/heads/main/security/evari-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Australia
- Insurtech
- Policy Administration
- Core Systems
- Property and Casualty
- Underwriting
- Claims
- Brokers
- MGA
- Artificial Intelligence
- Quoting
- Endorsements
---
