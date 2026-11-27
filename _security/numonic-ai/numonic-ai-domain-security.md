---
api_specs:
- filename: numonic-ai-openapi-generated.yml
  format: yaml
  label: Numonic Ltd. API
  slug: numonic-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/numonic-ai/openapi/_ae-authored/numonic-ai-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:security@numonic.ai"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: numonic.ai
  spf: true
hosts:
- cert_expires: Feb  6 20:06:07 2027 GMT
  host: numonic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Numonic Ltd. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Numonic Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Numonic Ltd.
provider_slug: numonic-ai
slug: numonic-ai-domain-security
source_filename: numonic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numonic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 20:06:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: numonic.ai\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:security@numonic.ai\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/numonic-ai/security/numonic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Asset Management
- AI Generation
- Creative Studios
- Compliance
- Workflow Capture
- Midjourney
- ComfyUI
---
