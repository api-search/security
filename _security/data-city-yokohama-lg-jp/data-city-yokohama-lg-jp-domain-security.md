---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: lg.jp
  spf: false
hosts:
- cert_expires: Sep 17 08:02:04 2026 GMT
  host: data.city.yokohama.lg.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data City Yokohama Lg Jp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yokohama City Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Yokohama City Open Data
provider_slug: data-city-yokohama-lg-jp
slug: data-city-yokohama-lg-jp-domain-security
source_filename: data-city-yokohama-lg-jp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.city.yokohama.lg.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:02:04 2026 GMT\n  hsts: false\ndomains:\n- domain: lg.jp\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-city-yokohama-lg-jp/refs/heads/main/security/data-city-yokohama-lg-jp-domain-security.yml
summary_line: TLSv1.3
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- Japan
---
