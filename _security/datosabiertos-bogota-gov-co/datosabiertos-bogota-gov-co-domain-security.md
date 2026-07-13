---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bogota.gov.co
  spf: false
hosts:
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: datosabiertos.bogota.gov.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datosabiertos Bogota Gov Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datos Abiertos Bogota, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Datos Abiertos Bogota
provider_slug: datosabiertos-bogota-gov-co
slug: datosabiertos-bogota-gov-co-domain-security
source_filename: datosabiertos-bogota-gov-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datosabiertos.bogota.gov.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bogota.gov.co\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datosabiertos-bogota-gov-co/refs/heads/main/security/datosabiertos-bogota-gov-co-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Colombia
---
