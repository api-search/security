---
api_specs:
- filename: monerium-openapi.yml
  format: yaml
  label: Monerium API
  slug: monerium-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/monerium/openapi/monerium-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monerium.com
  spf: true
hosts:
- cert_expires: Jan 19 17:38:20 2027 GMT
  host: monerium.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Monerium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Monerium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Monerium
provider_slug: monerium
slug: monerium-domain-security
source_filename: monerium-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monerium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 17:38:20 2027 GMT\n  hsts: false\ndomains:\n- domain: monerium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/monerium/security/monerium-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- FinTech
- Payments
- Blockchain
- DigitalCurrency
- RegulatedMoney
---
