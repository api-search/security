---
api_specs:
- filename: schwarz-it-health-probe-api-openapi.yml
  format: yaml
  label: Schwarz IT Health Probe API
  slug: schwarz-it-health-probe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/openapi/schwarz-it-health-probe-api-openapi.yml
- filename: schwarz-it-lintings-api-openapi.yml
  format: yaml
  label: Schwarz IT Lintings API
  slug: schwarz-it-lintings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/openapi/schwarz-it-lintings-api-openapi.yml
- filename: schwarz-it-rules-api-openapi.yml
  format: yaml
  label: Schwarz IT Rules API
  slug: schwarz-it-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/openapi/schwarz-it-rules-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: jobs.schwarz
  spf: true
hosts:
- cert_expires: Dec 13 07:31:21 2026 GMT
  host: jobs.schwarz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Schwarz It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Schwarz IT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Schwarz IT
provider_slug: schwarz-it
slug: schwarz-it-domain-security
source_filename: schwarz-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jobs.schwarz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:31:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jobs.schwarz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/schwarz-it/refs/heads/main/security/schwarz-it-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API Governance
- API Linting
- Spectral
- OpenAPI
- Retail
- Germany
---
