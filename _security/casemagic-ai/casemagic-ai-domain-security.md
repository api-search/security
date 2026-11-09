---
api_specs:
- filename: casemagic-ai-cases-api-openapi.yml
  format: yaml
  label: CaseMagic Cases API
  slug: casemagic-ai-cases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casemagic-ai/openapi/casemagic-ai-cases-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: casemagic.ai
  spf: true
hosts:
- cert_expires: Dec 17 01:12:14 2026 GMT
  host: casemagic.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Casemagic Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CaseMagic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CaseMagic
provider_slug: casemagic-ai
slug: casemagic-ai-domain-security
source_filename: casemagic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: casemagic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 01:12:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: casemagic.ai\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/casemagic-ai/security/casemagic-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Court Data
- Alerts
- Free
---
