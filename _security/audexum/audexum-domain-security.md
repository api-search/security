---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: audexum.com
  spf: true
hosts:
- cert_expires: Aug 21 07:44:58 2026 GMT
  host: audexum.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Audexum Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Audexum, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Audexum
provider_slug: audexum
slug: audexum-domain-security
source_filename: audexum-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: audexum.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 07:44:58 2026 GMT\n  hsts: null\ndomains:\n- domain: audexum.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/audexum/refs/heads/main/security/audexum-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Text Analysis
- Public APIs
---
