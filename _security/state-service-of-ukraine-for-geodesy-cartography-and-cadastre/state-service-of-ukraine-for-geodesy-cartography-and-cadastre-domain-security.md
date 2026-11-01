---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: land.gov.ua
  spf: true
hosts:
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: land.gov.ua
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: State Service Of Ukraine For Geodesy Cartography And Cadastre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for State Service of Ukraine for Geodesy, Cartography and Cadastre, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: State Service of Ukraine for Geodesy, Cartography and Cadastre
provider_slug: state-service-of-ukraine-for-geodesy-cartography-and-cadastre
slug: state-service-of-ukraine-for-geodesy-cartography-and-cadastre-domain-security
source_filename: state-service-of-ukraine-for-geodesy-cartography-and-cadastre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: land.gov.ua\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: land.gov.ua\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/state-service-of-ukraine-for-geodesy-cartography-and-cadastre/security/state-service-of-ukraine-for-geodesy-cartography-and-cadastre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Geospatial
- GIS
- Cadastral
- Mapping
---
