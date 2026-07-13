---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: misiones.gov.ar
  spf: true
hosts:
- host: www.datos.misiones.gov.ar
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''www.datos.m'
kind: domain-security
layout: security
method: probed
name: Datos Misiones Gov Ar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for datos.misiones.gov.ar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: datos.misiones.gov.ar
provider_slug: datos-misiones-gov-ar
slug: datos-misiones-gov-ar-domain-security
source_filename: datos-misiones-gov-ar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.datos.misiones.gov.ar\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''www.datos.m'\n  hsts: null\ndomains:\n- domain: misiones.gov.ar\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datos-misiones-gov-ar/refs/heads/main/security/datos-misiones-gov-ar-domain-security.yml
summary_line: DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Argentina
---
