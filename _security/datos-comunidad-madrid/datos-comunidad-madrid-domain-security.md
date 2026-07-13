---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: comunidad.madrid
  spf: true
hosts:
- cert_expires: Aug 12 07:51:05 2026 GMT
  host: datos.comunidad.madrid
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datos Comunidad Madrid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Madrid Region Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Madrid Region Open Data
provider_slug: datos-comunidad-madrid
slug: datos-comunidad-madrid-domain-security
source_filename: datos-comunidad-madrid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.comunidad.madrid\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 07:51:05 2026 GMT\n  hsts: null\ndomains:\n- domain: comunidad.madrid\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-comunidad-madrid/refs/heads/main/security/datos-comunidad-madrid-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Spain
---
