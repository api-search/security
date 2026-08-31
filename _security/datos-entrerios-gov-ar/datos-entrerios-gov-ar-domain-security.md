---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: entrerios.gov.ar
  spf: true
hosts:
- cert_expires: Sep 22 09:25:16 2026 GMT
  host: datos.entrerios.gov.ar
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datos Entrerios Gov Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Entre Rios Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Entre Rios Open Data
provider_slug: datos-entrerios-gov-ar
slug: datos-entrerios-gov-ar-domain-security
source_filename: datos-entrerios-gov-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.entrerios.gov.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 09:25:16 2026 GMT\n  hsts: false\ndomains:\n- domain: entrerios.gov.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-entrerios-gov-ar/refs/heads/main/security/datos-entrerios-gov-ar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Argentina
---
