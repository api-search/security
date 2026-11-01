---
api_specs:
- filename: seaweb-tech-openapi-generated.yml
  format: yaml
  label: seaweb-tech API
  slug: seaweb-tech-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/seaweb-tech/openapi/_ae-authored/seaweb-tech-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: seaweb.tech
  spf: false
hosts:
- cert_expires: Nov 28 07:30:45 2026 GMT
  host: seaweb.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Seaweb Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for seaweb-tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: seaweb-tech
provider_slug: seaweb-tech
slug: seaweb-tech-domain-security
source_filename: seaweb-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: seaweb.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 07:30:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: seaweb.tech\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/seaweb-tech/security/seaweb-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- AI
- ContextAPI
- Search
- Extraction
- Monitoring
---
