---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gub.uy
  spf: false
hosts:
- host: catalogodatos.gub.uy
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate in certificate chain (_ssl.c:1082)'
kind: domain-security
layout: security
method: probed
name: Catalogodatos Gub Uy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for datos.gub.uy - Catálogo de Datos Abiertos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: datos.gub.uy - Catálogo de Datos Abiertos
provider_slug: catalogodatos-gub-uy
slug: catalogodatos-gub-uy-domain-security
source_filename: catalogodatos-gub-uy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalogodatos.gub.uy\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: self-signed certificate\n    in certificate chain (_ssl.c:1082)'\n  hsts: null\ndomains:\n- domain: gub.uy\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catalogodatos-gub-uy/refs/heads/main/security/catalogodatos-gub-uy-domain-security.yml
summary_line: DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- International
---
