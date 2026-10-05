---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blankbeauty.com
  spf: true
hosts:
- cert_expires: Nov 11 20:00:01 2026 GMT
  host: blankbeauty.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blank Beauty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blank Beauty, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Blank Beauty
provider_slug: blank-beauty
slug: blank-beauty-domain-security
source_filename: blank-beauty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blankbeauty.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 20:00:01 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: blankbeauty.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blank-beauty/refs/heads/main/security/blank-beauty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Beauty
- NailPolish
- E-Commerce
- Vegan
---
