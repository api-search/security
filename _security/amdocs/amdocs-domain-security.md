---
api_specs:
- filename: amdocs-connectx-openapi.yml
  format: yaml
  label: Amdocs connectX BSS API
  slug: amdocs-connectx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/openapi/amdocs-connectx-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amdocs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: amdocs-dbs.com
  spf: true
hosts:
- cert_expires: Nov  5 23:59:59 2026 GMT
  host: www.amdocs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 14 23:59:59 2027 GMT
  host: devportal.amdocs-dbs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.amdocs-dbs.com
  https: false
kind: domain-security
layout: security
method: probed
name: Amdocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amdocs, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Amdocs
provider_slug: amdocs
slug: amdocs-domain-security
source_filename: amdocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amdocs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: devportal.amdocs-dbs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 23:59:59 2027 GMT\n  hsts: false\n- host: api.amdocs-dbs.com\n  https: false\ndomains:\n- domain: amdocs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: amdocs-dbs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amdocs/refs/heads/main/security/amdocs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Telecom
- BSS
- OSS
- Billing
- Customer Management
- MVNO
- 5G
- SaaS
---
