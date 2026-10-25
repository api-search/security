---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: translink.com.au
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: translink.com.au
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Translink Queensland Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Translink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Translink
provider_slug: translink-queensland
slug: translink-queensland-domain-security
source_filename: translink-queensland-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: translink.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: translink.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/translink-queensland/refs/heads/main/security/translink-queensland-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Public Transport
- Transit
- GTFS
- GTFS Realtime
- Open Data
- Government
- Queensland
- Australia
---
