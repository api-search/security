---
api_specs:
- filename: theta-lake-openapi-original.yml
  format: yaml
  label: Theta Lake API
  slug: theta-lake-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/theta-lake/refs/heads/main/openapi/theta-lake-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thetalake.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: thetalake.ai
  spf: true
hosts:
- cert_expires: Oct  8 15:23:47 2026 GMT
  host: thetalake.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: developer.thetalake.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Theta Lake Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Theta Lake, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Theta Lake
provider_slug: theta-lake
slug: theta-lake-domain-security
source_filename: theta-lake-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetalake.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 15:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.thetalake.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thetalake.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: thetalake.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/theta-lake/refs/heads/main/security/theta-lake-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Communications Governance
- Compliance
- Archiving
- Security
- Supervision
- eDiscovery
- Legal Hold
- Records Management
- Unified Communications
- AI Governance
- Regulatory Compliance
---
