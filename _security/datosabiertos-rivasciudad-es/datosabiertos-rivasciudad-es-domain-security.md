---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rivasciudad.es
  spf: true
hosts:
- cert_expires: Oct  6 08:11:43 2026 GMT
  host: datosabiertos.rivasciudad.es
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datosabiertos Rivasciudad Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Portal oficial Ayuntamiento de Rivas Vaciamadrid, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Portal oficial Ayuntamiento de Rivas Vaciamadrid
provider_slug: datosabiertos-rivasciudad-es
slug: datosabiertos-rivasciudad-es-domain-security
source_filename: datosabiertos-rivasciudad-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datosabiertos.rivasciudad.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 08:11:43 2026 GMT\n  hsts: false\ndomains:\n- domain: rivasciudad.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datosabiertos-rivasciudad-es/refs/heads/main/security/datosabiertos-rivasciudad-es-domain-security.yml
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
