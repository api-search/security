---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opendata-hro.de
  spf: false
hosts:
- cert_expires: Jan 20 00:11:40 2027 GMT
  host: www.opendata-hro.de
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Hro De Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenData.HRO - Portal für offene Data der Hansestadt Rostock, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenData.HRO - Portal für offene Data der Hansestadt Rostock
provider_slug: opendata-hro-de
slug: opendata-hro-de-domain-security
source_filename: opendata-hro-de-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opendata-hro.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 00:11:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: opendata-hro.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-hro-de/refs/heads/main/security/opendata-hro-de-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Germany
---
