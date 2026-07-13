---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 iodef "mailto:abuse@upm.es"
  - 0 issue "digicert.com"
  - 0 issue "fnmt.es"
  - 0 issue "harica.gr"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: upm.es
  spf: true
hosts:
- cert_expires: Nov  7 11:57:39 2026 GMT
  host: portal-yoda.dit.upm.es
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Portal Yoda Dit Upm Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UPM YODA Open Data Portal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: UPM YODA Open Data Portal
provider_slug: portal-yoda-dit-upm-es
slug: portal-yoda-dit-upm-es-domain-security
source_filename: portal-yoda-dit-upm-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal-yoda.dit.upm.es\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  7 11:57:39 2026 GMT\n  hsts: false\ndomains:\n- domain: upm.es\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 iodef \"mailto:abuse@upm.es\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"fnmt.es\"\n  - 0 issue \"harica.gr\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/portal-yoda-dit-upm-es/refs/heads/main/security/portal-yoda-dit-upm-es-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- University Data
- University
- Spain
---
