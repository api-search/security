---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: friendlydata.io
  spf: true
hosts:
- cert_expires: Aug 30 15:40:00 2026 GMT
  host: friendlydata.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Friendly Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Friendly Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Friendly Data
provider_slug: friendly-data
slug: friendly-data-domain-security
source_filename: friendly-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: friendlydata.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 15:40:00 2026 GMT\n  hsts: null\ndomains:\n- domain: friendlydata.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/friendly-data/refs/heads/main/security/friendly-data-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
