---
api_specs:
- filename: acruxcore-account-api-openapi.yml
  format: yaml
  label: Acrux Core Account API
  slug: acruxcore-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/acruxcore-account-api-openapi.yml
- filename: acruxcore-acrux-core-api-api-openapi.yml
  format: yaml
  label: Acrux Core Acrux Core API
  slug: acruxcore-acrux-core-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/acruxcore-acrux-core-api-api-openapi.yml
- filename: acruxcore-prompts-api-openapi.yml
  format: yaml
  label: Acrux Core Prompts API
  slug: acruxcore-prompts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/acruxcore-prompts-api-openapi.yml
- filename: acruxcore-tools-api-openapi.yml
  format: yaml
  label: Acrux Core Tools API
  slug: acruxcore-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/acruxcore-tools-api-openapi.yml
- filename: acruxcore-traces-api-openapi.yml
  format: yaml
  label: Acrux Core Traces API
  slug: acruxcore-traces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/openapi/acruxcore-traces-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: acruxcore.com
  spf: true
hosts:
- cert_expires: Dec  9 18:39:44 2026 GMT
  host: acruxcore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Acruxcore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acrux Core, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Acrux Core
provider_slug: acruxcore
slug: acruxcore-domain-security
source_filename: acruxcore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: acruxcore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 18:39:44 2026 GMT\n  hsts: false\ndomains:\n- domain: acruxcore.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acruxcore/refs/heads/main/security/acruxcore-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- LLMOps
- Open Source
- Platform
- Engineering
- Artificial Intelligence
---
