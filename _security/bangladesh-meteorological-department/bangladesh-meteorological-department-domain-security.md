---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bmd.gov.bd
  spf: true
hosts:
- cert_expires: May  1 23:59:59 2027 GMT
  host: bmd.gov.bd
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bangladesh Meteorological Department Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BMD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BMD
provider_slug: bangladesh-meteorological-department
slug: bangladesh-meteorological-department-domain-security
source_filename: bangladesh-meteorological-department-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bmd.gov.bd\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bmd.gov.bd\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bangladesh-meteorological-department/security/bangladesh-meteorological-department-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Weather
- Climate
- Government
- Data
---
