---
api_specs:
- filename: ambitioninc-account-api-openapi.yml
  format: yaml
  label: Ambitioninc Account API
  slug: ambitioninc-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambitioninc/refs/heads/main/openapi/ambitioninc-account-api-openapi.yml
- filename: ambitioninc-data-api-openapi.yml
  format: yaml
  label: Ambitioninc Data API
  slug: ambitioninc-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ambitioninc/refs/heads/main/openapi/ambitioninc-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ambition.com
  spf: true
hosts:
- cert_expires: Nov 17 20:16:58 2026 GMT
  host: ambition.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ambitioninc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ambitioninc, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ambitioninc
provider_slug: ambitioninc
slug: ambitioninc-domain-security
source_filename: ambitioninc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ambition.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 20:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ambition.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambitioninc/refs/heads/main/security/ambitioninc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Software-as-a-Service
- Revenue Operations
- Sales Enablement
- Artificial Intelligence
- Platform
---
