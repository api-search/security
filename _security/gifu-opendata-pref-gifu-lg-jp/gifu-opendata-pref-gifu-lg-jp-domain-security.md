---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lg.jp
  spf: false
hosts:
- cert_expires: Oct 27 08:34:49 2026 GMT
  host: gifu-opendata.pref.gifu.lg.jp
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gifu Opendata Pref Gifu Lg Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gifu Prefecture Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Gifu Prefecture Open Data
provider_slug: gifu-opendata-pref-gifu-lg-jp
slug: gifu-opendata-pref-gifu-lg-jp-domain-security
source_filename: gifu-opendata-pref-gifu-lg-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gifu-opendata.pref.gifu.lg.jp\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 27 08:34:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lg.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gifu-opendata-pref-gifu-lg-jp/refs/heads/main/security/gifu-opendata-pref-gifu-lg-jp-domain-security.yml
summary_line: TLSv1.2 · HSTS
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Regional Government
- Japan
---
