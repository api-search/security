---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opendata.gov.je
  spf: false
hosts:
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: opendata.gov.je
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Gov Je Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for opendata.gov.je, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: opendata.gov.je
provider_slug: opendata-gov-je
slug: opendata-gov-je-domain-security
source_filename: opendata-gov-je-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.gov.je\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: opendata.gov.je\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-gov-je/refs/heads/main/security/opendata-gov-je-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- JE
---
