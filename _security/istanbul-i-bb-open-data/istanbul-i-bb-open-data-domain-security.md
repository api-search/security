---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ibb.gov.tr
  spf: false
hosts:
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: data.ibb.gov.tr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Istanbul I Bb Open Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Istanbul (İBB) Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Istanbul (İBB) Open Data
provider_slug: istanbul-i-bb-open-data
slug: istanbul-i-bb-open-data-domain-security
source_filename: istanbul-i-bb-open-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.ibb.gov.tr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ibb.gov.tr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istanbul-i-bb-open-data/refs/heads/main/security/istanbul-i-bb-open-data-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Government
- Public APIs
---
