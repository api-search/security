---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: imd.gov.in
  spf: true
hosts:
- cert_expires: Jan 13 09:08:58 2027 GMT
  host: mausam.imd.gov.in
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 13 09:08:58 2027 GMT
  host: api.imd.gov.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: India Meteorological Department Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for India Meteorological Department, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: India Meteorological Department
provider_slug: india-meteorological-department
slug: india-meteorological-department-domain-security
source_filename: india-meteorological-department-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mausam.imd.gov.in\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 13 09:08:58 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.imd.gov.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 09:08:58 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: imd.gov.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/india-meteorological-department/security/india-meteorological-department-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Weather
- Meteorology
- India
- Public-Data
- Climate
- Government
---
