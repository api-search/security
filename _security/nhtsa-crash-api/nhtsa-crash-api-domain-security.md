---
api_specs:
- filename: nhtsa-crash-api-nhtsa-crash-data-api-openapi.yml
  format: yaml
  label: NHTSA Crash Data API
  slug: nhtsa-crash-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nhtsa-crash-api/refs/heads/main/openapi/nhtsa-crash-api-nhtsa-crash-data-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: nhtsa.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dot.gov
  spf: true
hosts:
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: www.nhtsa.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: crashviewer.nhtsa.dot.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nhtsa Crash Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NHTSA Crash API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: NHTSA Crash API
provider_slug: nhtsa-crash-api
slug: nhtsa-crash-api-domain-security
source_filename: nhtsa-crash-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nhtsa.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\n- host: crashviewer.nhtsa.dot.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: nhtsa.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dot.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nhtsa-crash-api/refs/heads/main/security/nhtsa-crash-api-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Crash Data
- Government
- NHTSA
- Traffic Safety
- Transportation
---
