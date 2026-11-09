---
api_specs:
- filename: 5arz-com-api-openapi.json
  format: json
  label: 5arz Proof-of-Human API API
  slug: 5arz-proof-of-human-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/5arz-com/openapi/_original/5arz-com-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: 5arz.com
  spf: true
hosts:
- cert_expires: Dec 29 23:20:53 2026 GMT
  host: 5arz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 5Arz Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 5arz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: 5arz
provider_slug: 5arz-com
slug: 5arz-com-domain-security
source_filename: 5arz-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 5arz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:20:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: 5arz.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/5arz-com/security/5arz-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Human Verification
- Artificial Intelligence
- Privacy
- Developer Tools
- Authentication
---
