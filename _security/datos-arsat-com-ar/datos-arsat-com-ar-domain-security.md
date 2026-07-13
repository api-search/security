---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: arsat.com.ar
  spf: true
hosts:
- cert_expires: Aug  8 23:59:59 2026 GMT
  host: datos.arsat.com.ar
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datos Arsat Com Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datos Abiertos ARSAT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Datos Abiertos ARSAT
provider_slug: datos-arsat-com-ar
slug: datos-arsat-com-ar-domain-security
source_filename: datos-arsat-com-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datos.arsat.com.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  8 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: arsat.com.ar\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-arsat-com-ar/refs/heads/main/security/datos-arsat-com-ar-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Argentina
---
