---
api_specs:
- filename: unitrends-public-api-openapi.json
  format: json
  label: Unitrends MSP Public API (UniView Portal)
  slug: unitrends-msp-public-api-uniview-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/openapi/unitrends-public-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unitrends.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: backup.net
  spf: false
hosts:
- cert_expires: Sep  8 21:03:53 2026 GMT
  host: www.unitrends.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: apidoc-public-api.backup.net
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: public-api.backup.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Unitrends Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Unitrends, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Unitrends
provider_slug: unitrends
slug: unitrends-domain-security
source_filename: unitrends-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.unitrends.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 21:03:53 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: apidoc-public-api.backup.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: public-api.backup.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: unitrends.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: backup.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitrends/refs/heads/main/security/unitrends-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Backup
- Disaster Recovery
- Data Protection
- BCDR
- Ransomware Protection
- MSP
- Endpoint Backup
---
