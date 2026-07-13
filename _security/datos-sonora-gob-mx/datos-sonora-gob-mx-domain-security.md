---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gob.mx
  spf: true
hosts:
- cert_expires: Feb 23 20:35:31 2027 GMT
  host: datos.sonora.gob.mx
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datos Sonora Gob Mx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sonora Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Sonora Open Data
provider_slug: datos-sonora-gob-mx
slug: datos-sonora-gob-mx-domain-security
source_filename: datos-sonora-gob-mx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.sonora.gob.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 20:35:31 2027 GMT\n  hsts: null\ndomains:\n- domain: gob.mx\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-sonora-gob-mx/refs/heads/main/security/datos-sonora-gob-mx-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- State Government
- Mexico
---
