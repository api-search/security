---
api_specs:
- filename: machina-gg-forecast-signals-api-openapi.yml
  format: yaml
  label: Machina Sports Forecast Signals API
  slug: machina-gg-forecast-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-forecast-signals-api-openapi.yml
- filename: machina-gg-intelligence-api-openapi.yml
  format: yaml
  label: Machina Sports Intelligence API
  slug: machina-gg-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-intelligence-api-openapi.yml
- filename: machina-gg-markets-api-openapi.yml
  format: yaml
  label: Machina Sports Markets API
  slug: machina-gg-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-markets-api-openapi.yml
- filename: machina-gg-match-context-api-openapi.yml
  format: yaml
  label: Machina Sports Match Context API
  slug: machina-gg-match-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-match-context-api-openapi.yml
- filename: machina-gg-skills-api-openapi.yml
  format: yaml
  label: Machina Sports Skills API
  slug: machina-gg-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-skills-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: machina.gg
  spf: true
hosts:
- cert_expires: May  4 23:59:59 2027 GMT
  host: machina.gg
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Machina Sports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Machina Sports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Machina Sports
provider_slug: machina-gg
slug: machina-gg-domain-security
source_filename: machina-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: machina.gg\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  4 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: machina.gg\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/machina-gg/security/machina-gg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Sports
- Artificial Intelligence
- Platform
- Sports AI
- Developers
---
