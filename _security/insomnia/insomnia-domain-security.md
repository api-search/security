---
api_specs:
- filename: insomnia-mock-logs-api-openapi.yml
  format: yaml
  label: Insomnia Mock Logs API
  slug: insomnia-mock-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-logs-api-openapi.yml
- filename: insomnia-mock-routes-api-openapi.yml
  format: yaml
  label: Insomnia Mock Routes API
  slug: insomnia-mock-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-routes-api-openapi.yml
- filename: insomnia-mock-servers-api-openapi.yml
  format: yaml
  label: Insomnia Mock Servers API
  slug: insomnia-mock-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/openapi/insomnia-mock-servers-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: insomnia.rest
  spf: true
hosts:
- cert_expires: Nov 30 08:35:23 2026 GMT
  host: insomnia.rest
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 29 00:50:39 2026 GMT
  host: mock.insomnia.rest
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Insomnia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Insomnia, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Insomnia
provider_slug: insomnia
slug: insomnia-domain-security
source_filename: insomnia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insomnia.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 08:35:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mock.insomnia.rest\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 00:50:39 2026 GMT\n  hsts: null\ndomains:\n- domain: insomnia.rest\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/insomnia/refs/heads/main/security/insomnia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Design
- CLI
- Clients
- Developer Tools
- Mocking
- Platform
- Testing
- OpenAPI
---
