---
api_specs:
- filename: autify-autify-cli-api-openapi.yml
  format: yaml
  label: Autify Autify Cli API
  slug: autify-autify-cli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autify/refs/heads/main/openapi/autify-autify-cli-api-openapi.yml
- filename: autify-default-api-openapi.yml
  format: yaml
  label: Autify ~ API
  slug: autify-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autify/refs/heads/main/openapi/autify-default-api-openapi.yml
- filename: autify-payload-api-openapi.yml
  format: yaml
  label: Autify Payload API
  slug: autify-payload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autify/refs/heads/main/openapi/autify-payload-api-openapi.yml
- filename: autify-projects-api-openapi.yml
  format: yaml
  label: Autify Projects API
  slug: autify-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autify/refs/heads/main/openapi/autify-projects-api-openapi.yml
- filename: autify-workspaces-api-openapi.yml
  format: yaml
  label: Autify Workspaces API
  slug: autify-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autify/refs/heads/main/openapi/autify-workspaces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: autify.com
  spf: true
hosts:
- cert_expires: Dec 12 15:25:18 2026 GMT
  host: autify.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Autify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Autify
provider_slug: autify
slug: autify-domain-security
source_filename: autify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 15:25:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: autify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autify/refs/heads/main/security/autify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Test Automation
- No-Code
- Software-as-a-Service
---
