---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: toscana.it
  spf: false
hosts:
- host: dati.lamma.toscana.it
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get local issuer certificate (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Dati Lamma Toscana It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LAMMA Toscana Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: LAMMA Toscana Open Data
provider_slug: dati-lamma-toscana-it
slug: dati-lamma-toscana-it-domain-security
source_filename: dati-lamma-toscana-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.lamma.toscana.it\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: unable to get\n    local issuer certificate (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: toscana.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-lamma-toscana-it/refs/heads/main/security/dati-lamma-toscana-it-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Government Agency
- Italy
---
