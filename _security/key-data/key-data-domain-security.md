---
api_specs:
- filename: key-data-key-data-api-api-openapi.yml
  format: yaml
  label: Key Data API
  slug: key-data-api-2
  spec_type: OpenAPI
  url: https://artifacts.apis.io/key-data/openapi/key-data-key-data-api-api-openapi.yml
- filename: key-data-openapi-generated.yml
  format: yaml
  label: Key Data API
  slug: key-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/key-data/openapi/_ae-authored/key-data-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keydata.co
  spf: true
hosts:
- cert_expires: Dec 13 01:25:13 2026 GMT
  host: keydata.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Key Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Key Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Key Data
provider_slug: key-data
slug: key-data-domain-security
source_filename: key-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keydata.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 01:25:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keydata.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/key-data/security/key-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- short-term rentals
- real-time data
- analytics
- property management
- vacation rentals
---
