---
api_specs:
- filename: deck-connection-api-openapi.yml
  format: yaml
  label: Deck Connection API
  slug: deck-connection-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deck/openapi/deck-connection-api-openapi.yml
- filename: deck-jobs-api-openapi.yml
  format: yaml
  label: Deck Jobs API
  slug: deck-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deck/openapi/deck-jobs-api-openapi.yml
- filename: deck-link-api-openapi.yml
  format: yaml
  label: Deck Link API
  slug: deck-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/deck/openapi/deck-link-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: deck.co
  spf: true
hosts:
- cert_expires: Dec 11 21:45:54 2026 GMT
  host: deck.co
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Deck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Deck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Deck
provider_slug: deck
slug: deck-domain-security
source_filename: deck-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deck.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 21:45:54 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: deck.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/deck/security/deck-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automation
- API Integration
- Enterprise
- Security
---
