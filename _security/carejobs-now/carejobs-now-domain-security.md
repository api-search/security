---
api_specs:
- filename: carejobs-now-pay-api-openapi.yml
  format: yaml
  label: CareJobs.Now Pay API
  slug: carejobs-now-pay-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carejobs-now/refs/heads/main/openapi/carejobs-now-pay-api-openapi.yml
- filename: carejobs-now-roles-api-openapi.yml
  format: yaml
  label: CareJobs.Now Roles API
  slug: carejobs-now-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/carejobs-now/refs/heads/main/openapi/carejobs-now-roles-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carejobs.now
  spf: false
hosts:
- cert_expires: Jan  4 17:58:39 2027 GMT
  host: carejobs.now
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carejobs Now Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CareJobs.Now, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: CareJobs.Now
provider_slug: carejobs-now
slug: carejobs-now-domain-security
source_filename: carejobs-now-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carejobs.now\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 17:58:39 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carejobs.now\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carejobs-now/refs/heads/main/security/carejobs-now-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- Job
- Data
- Transparency
- US
---
