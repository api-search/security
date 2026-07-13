---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: modena.it
  spf: false
hosts:
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: opendata.comune.modena.it
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opendata Comune Modena It Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Modena Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Modena Open Data
provider_slug: opendata-comune-modena-it
slug: opendata-comune-modena-it-domain-security
source_filename: opendata-comune-modena-it-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.comune.modena.it\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: modena.it\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-comune-modena-it/refs/heads/main/security/opendata-comune-modena-it-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Municipal Government
- Italy
---
