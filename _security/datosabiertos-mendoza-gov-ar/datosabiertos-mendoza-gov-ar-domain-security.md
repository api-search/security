---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mendoza.gov.ar
  spf: true
hosts:
- cert_expires: Jul 28 17:17:19 2026 GMT
  host: datosabiertos.mendoza.gov.ar
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Datosabiertos Mendoza Gov Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mendoza Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mendoza Open Data
provider_slug: datosabiertos-mendoza-gov-ar
slug: datosabiertos-mendoza-gov-ar-domain-security
source_filename: datosabiertos-mendoza-gov-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datosabiertos.mendoza.gov.ar\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 17:17:19 2026 GMT\n  hsts: false\ndomains:\n- domain: mendoza.gov.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datosabiertos-mendoza-gov-ar/refs/heads/main/security/datosabiertos-mendoza-gov-ar-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- State Government
- Argentina
---
