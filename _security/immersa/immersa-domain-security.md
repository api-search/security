---
api_specs:
- filename: immersa-openapi-generated.yml
  format: yaml
  label: Immersa API
  slug: immersa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immersa/refs/heads/main/openapi/_ae-authored/immersa-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: immersa.ai
  spf: true
hosts:
- cert_expires: Nov 26 10:20:09 2026 GMT
  host: immersa.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Immersa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Immersa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Immersa
provider_slug: immersa
slug: immersa-domain-security
source_filename: immersa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: immersa.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 10:20:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: immersa.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immersa/refs/heads/main/security/immersa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- DataGateway
- Platform
- Security
---
