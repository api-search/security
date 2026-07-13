---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aragon.es
  spf: true
hosts:
- cert_expires: Mar 21 16:21:13 2027 GMT
  host: opendata.aragon.es
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Opendata Aragon Es Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aragón Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aragón Open Data
provider_slug: opendata-aragon-es
slug: opendata-aragon-es-domain-security
source_filename: opendata-aragon-es-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.aragon.es\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 21 16:21:13 2027 GMT\n  hsts: false\ndomains:\n- domain: aragon.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opendata-aragon-es/refs/heads/main/security/opendata-aragon-es-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Open Data Portal
- Spain
---
