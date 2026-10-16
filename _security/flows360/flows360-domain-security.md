---
api_specs:
- filename: flows360-openapi-generated.yml
  format: yaml
  label: Flows360 API
  slug: flows360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flows360/refs/heads/main/openapi/_ae-authored/flows360-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flows360.co
  spf: false
hosts:
- cert_expires: Dec 26 14:34:53 2026 GMT
  host: flows360.co
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flows360 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flows360, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Flows360
provider_slug: flows360
slug: flows360-domain-security
source_filename: flows360-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flows360.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 14:34:53 2026 GMT\n  hsts: false\ndomains:\n- domain: flows360.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flows360/refs/heads/main/security/flows360-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automation
- Workflow
- Integration
- SaaS
---
