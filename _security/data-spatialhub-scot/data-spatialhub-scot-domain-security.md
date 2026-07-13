---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spatialhub.scot
  spf: false
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: data.spatialhub.scot
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Data Spatialhub Scot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spatial Hub Scotland, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Spatial Hub Scotland
provider_slug: data-spatialhub-scot
slug: data-spatialhub-scot-domain-security
source_filename: data-spatialhub-scot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.spatialhub.scot\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: spatialhub.scot\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-spatialhub-scot/refs/heads/main/security/data-spatialhub-scot-domain-security.yml
summary_line: TLSv1.2
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- United Kingdom
---
