---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lg.jp
  spf: false
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: catalog.data.metro.tokyo.lg.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Catalog Data Metro Tokyo Lg Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tokyo Metropolitan Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Tokyo Metropolitan Open Data
provider_slug: catalog-data-metro-tokyo-lg-jp
slug: catalog-data-metro-tokyo-lg-jp-domain-security
source_filename: catalog-data-metro-tokyo-lg-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: catalog.data.metro.tokyo.lg.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lg.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/catalog-data-metro-tokyo-lg-jp/refs/heads/main/security/catalog-data-metro-tokyo-lg-jp-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Japan
---
