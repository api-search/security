---
api_specs:
- filename: soccer-data-co-openapi-generated.yml
  format: yaml
  label: Soccer Data API
  slug: soccer-data-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/soccer-data-co/openapi/_ae-authored/soccer-data-co-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: soccer-data.co
  spf: false
hosts:
- cert_expires: Jan 26 19:43:56 2027 GMT
  host: soccer-data.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Soccer Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soccer Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Soccer Data
provider_slug: soccer-data-co
slug: soccer-data-co-domain-security
source_filename: soccer-data-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: soccer-data.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 26 19:43:56 2027 GMT\n  hsts: false\ndomains:\n- domain: soccer-data.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/soccer-data-co/security/soccer-data-co-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Football API
- Live Scores
- Odds
- Betting
- Fantasy Games
---
