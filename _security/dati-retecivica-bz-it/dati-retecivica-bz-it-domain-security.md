---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bz.it
  spf: false
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: dati.retecivica.bz.it
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dati Retecivica Bz It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for South Tyrol Retecivica Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: South Tyrol Retecivica Data
provider_slug: dati-retecivica-bz-it
slug: dati-retecivica-bz-it-domain-security
source_filename: dati-retecivica-bz-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.retecivica.bz.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bz.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-retecivica-bz-it/refs/heads/main/security/dati-retecivica-bz-it-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Italy
---
