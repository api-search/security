---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: minneapolismn.gov
  spf: true
hosts:
- cert_expires: Sep  7 11:28:49 2026 GMT
  host: opendata.minneapolismn.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Data Minneapolis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Data Minneapolis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Open Data Minneapolis
provider_slug: open-data-minneapolis
slug: open-data-minneapolis-domain-security
source_filename: open-data-minneapolis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opendata.minneapolismn.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:28:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: minneapolismn.gov\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-data-minneapolis/refs/heads/main/security/open-data-minneapolis-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- Public APIs
---
