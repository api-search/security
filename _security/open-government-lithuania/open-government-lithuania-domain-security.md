---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: data.gov.lt
  spf: true
hosts:
- cert_expires: May  2 23:59:59 2027 GMT
  host: data.gov.lt
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lithuanian Open Data Portal (data.gov.lt) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lithuanian Open Data Portal (data.gov.lt), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Lithuanian Open Data Portal (data.gov.lt)
provider_slug: open-government-lithuania
slug: open-government-lithuania-domain-security
source_filename: open-government-lithuania-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.gov.lt\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: data.gov.lt\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/open-government-lithuania/security/open-government-lithuania-domain-security.yml
summary_line: TLSv1.3
tags:
- Datasets
- Government
- Lithuania
- Open Data
- Public APIs
- Public Sector
- UAPI
---
