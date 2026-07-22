---
api_specs:
- filename: vectranetworks-rux-v3.3-openapi.yml
  format: yaml
  label: Vectra AI Platform API (RUX)
  slug: vectra-ai-platform-api-rux
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-rux-v3.3-openapi.yml
- filename: vectranetworks-detect-v2.3-openapi.yml
  format: yaml
  label: Vectra Detect API
  slug: vectra-detect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/openapi/vectranetworks-detect-v2.3-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: vectra.ai
  spf: true
hosts:
- cert_expires: Oct  2 15:47:38 2026 GMT
  host: www.vectra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: platform.vectra.ai
  https: false
kind: domain-security
layout: security
method: probed
name: Vectranetworks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vectra AI, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Vectra AI
provider_slug: vectranetworks
slug: vectranetworks-domain-security
source_filename: vectranetworks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vectra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:47:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: platform.vectra.ai\n  https: false\ndomains:\n- domain: vectra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vectranetworks/refs/heads/main/security/vectranetworks-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Cybersecurity
- Network Detection and Response
- Threat Detection
- Security Operations
- Artificial Intelligence
- SIEM
---
