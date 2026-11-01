---
api_specs:
- filename: hubrise-openapi-generated.yml
  format: yaml
  label: HubRise API
  slug: hubrise-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubrise/openapi/_ae-authored/hubrise-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hubrise.com
  spf: true
hosts:
- cert_expires: Jan  1 23:45:15 2027 GMT
  host: hubrise.com
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hubrise Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HubRise, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: HubRise
provider_slug: hubrise
slug: hubrise-domain-security
source_filename: hubrise-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hubrise.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  1 23:45:15 2027 GMT\n  hsts: true\n  hsts_max_age: 15724800\ndomains:\n- domain: hubrise.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/hubrise/security/hubrise-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Integration
- Retail
- Hospitality
- API
---
