---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ugr.es
  spf: true
hosts:
- cert_expires: Sep  3 00:29:11 2026 GMT
  host: opendata.ugr.es
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Ugr Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bienvenido a OpenData UGR, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bienvenido a OpenData UGR
provider_slug: opendata-ugr-es
slug: opendata-ugr-es-domain-security
source_filename: opendata-ugr-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.ugr.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 00:29:11 2026 GMT\n  hsts: false\ndomains:\n- domain: ugr.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-ugr-es/refs/heads/main/security/opendata-ugr-es-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Spain
---
