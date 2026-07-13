---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: unibo.it
  spf: true
hosts:
- cert_expires: Aug 18 09:14:49 2026 GMT
  host: dati.unibo.it
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dati Unibo It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Bologna Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: University of Bologna Open Data
provider_slug: dati-unibo-it
slug: dati-unibo-it-domain-security
source_filename: dati-unibo-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dati.unibo.it\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 18 09:14:49 2026 GMT\n  hsts: false\ndomains:\n- domain: unibo.it\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dati-unibo-it/refs/heads/main/security/dati-unibo-it-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- University Data
- University
- Italy
---
