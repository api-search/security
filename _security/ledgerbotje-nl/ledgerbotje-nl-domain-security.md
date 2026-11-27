---
api_specs:
- filename: ledgerbotje-nl-app-api-openapi.yml
  format: yaml
  label: Ledger Botje App API
  slug: ledgerbotje-nl-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgerbotje-nl/openapi/ledgerbotje-nl-app-api-openapi.yml
- filename: ledgerbotje-nl-well-known-api-openapi.yml
  format: yaml
  label: Ledger Botje .well Known API
  slug: ledgerbotje-nl-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgerbotje-nl/openapi/ledgerbotje-nl-well-known-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ledgerbotje.nl
  spf: true
hosts:
- cert_expires: Dec 27 05:27:00 2026 GMT
  host: ledgerbotje.nl
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ledger Botje Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ledger Botje, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ledger Botje
provider_slug: ledgerbotje-nl
slug: ledgerbotje-nl-domain-security
source_filename: ledgerbotje-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ledgerbotje.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 05:27:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ledgerbotje.nl\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ledgerbotje-nl/security/ledgerbotje-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Accounting
- Artificial Intelligence
- Automation
- ExactOnline
- Netherlands
---
