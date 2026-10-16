---
api_specs:
- filename: askai-openapi-generated.yml
  format: yaml
  label: GPTfy API
  slug: askai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/askai/refs/heads/main/openapi/_ae-authored/askai-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: askai.free
  spf: false
hosts:
- cert_expires: Jan  4 19:04:48 2027 GMT
  host: askai.free
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Askai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GPTfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: GPTfy
provider_slug: askai
slug: askai-domain-security
source_filename: askai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askai.free\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 19:04:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: askai.free\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/askai/refs/heads/main/security/askai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Language-Model
- Platform
- API
---
