---
api_specs:
- filename: keenable-fetch-api-openapi.yml
  format: yaml
  label: Keenable Fetch API
  slug: keenable-fetch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenable/openapi/keenable-fetch-api-openapi.yml
- filename: keenable-search-api-openapi.yml
  format: yaml
  label: Keenable Search API
  slug: keenable-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keenable/openapi/keenable-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: keenable.ai
  spf: true
hosts:
- cert_expires: Jan 19 03:54:18 2027 GMT
  host: keenable.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keenable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keenable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Keenable
provider_slug: keenable
slug: keenable-domain-security
source_filename: keenable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keenable.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 03:54:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: keenable.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/keenable/security/keenable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Web Search
- API
- AI Agents
- AI Labs
- Inference Platforms
---
