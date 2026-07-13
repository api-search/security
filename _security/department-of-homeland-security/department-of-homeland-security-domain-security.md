---
api_specs:
- filename: department-of-homeland-security-openapi.yml
  format: yaml
  label: OpenFEMA API
  slug: openfema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-homeland-security/refs/heads/main/openapi/department-of-homeland-security-openapi.yml
description: ''
domains:
- caa:
  - ;; connection timed out; no servers could be reached
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dhs.gov
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fema.gov
  spf: true
hosts:
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.dhs.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 23:59:59 2026 GMT
  host: www.fema.gov
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: developer.uscis.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Department Of Homeland Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Department of Homeland Security, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Department of Homeland Security
provider_slug: department-of-homeland-security
slug: department-of-homeland-security-domain-security
source_filename: department-of-homeland-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dhs.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.fema.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 23:59:59 2026 GMT\n  hsts: null\n- host: developer.uscis.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dhs.gov\n  dnssec: true\n  caa:\n  - ;; connection timed out; no servers could be reached\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fema.gov\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-homeland-security/refs/heads/main/security/department-of-homeland-security-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CISA
- Cybersecurity
- Disaster
- Federal Government
- FEMA
- Homeland Security
- Immigration
- NTAS
- Open Data
- USCIS
---
