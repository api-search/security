---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: nla.gov.au
  spf: true
hosts:
- cert_expires: Oct  8 14:04:50 2026 GMT
  host: trove.nla.gov.au
  hsts: true
  hsts_max_age: 15811200
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trove Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trove, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Trove
provider_slug: trove
slug: trove-domain-security
source_filename: trove-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trove.nla.gov.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:04:50 2026 GMT\n  hsts: true\n  hsts_max_age: 15811200\ndomains:\n- domain: nla.gov.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trove/refs/heads/main/security/trove-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- News
- Public APIs
---
