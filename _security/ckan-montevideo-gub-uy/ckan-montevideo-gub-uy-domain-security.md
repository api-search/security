---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gub.uy
  spf: false
hosts:
- cert_expires: Nov 21 17:27:40 2026 GMT
  host: ckan.montevideo.gub.uy
  hsts: true
  hsts_max_age: 5184000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ckan Montevideo Gub Uy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Montevideo Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Montevideo Open Data
provider_slug: ckan-montevideo-gub-uy
slug: ckan-montevideo-gub-uy-domain-security
source_filename: ckan-montevideo-gub-uy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ckan.montevideo.gub.uy\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 17:27:40 2026 GMT\n  hsts: true\n  hsts_max_age: 5184000\ndomains:\n- domain: gub.uy\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ckan-montevideo-gub-uy/refs/heads/main/security/ckan-montevideo-gub-uy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Uruguay
---
