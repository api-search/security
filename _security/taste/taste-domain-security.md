---
api_specs:
- filename: taste-health-api-openapi.yml
  format: yaml
  label: Taste health API
  slug: taste-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/openapi/taste-health-api-openapi.yml
- filename: taste-prompt-enhancement-api-openapi.yml
  format: yaml
  label: Taste Prompt Enhancement API
  slug: taste-prompt-enhancement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/openapi/taste-prompt-enhancement-api-openapi.yml
- filename: taste-taste-engine-api-api-openapi.yml
  format: yaml
  label: Taste Taste Engine API API
  slug: taste-taste-engine-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/openapi/taste-taste-engine-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tastelabs.com
  spf: true
hosts:
- cert_expires: Sep 13 18:43:37 2026 GMT
  host: tastelabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Taste Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Taste, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Taste
provider_slug: taste
slug: taste-domain-security
source_filename: taste-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tastelabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:43:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: tastelabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taste/refs/heads/main/security/taste-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Design
- Machine-Learning
- Developer Tools
- Prompt Engineering
- Content Generation
---
