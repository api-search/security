---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: betterleap.com
  spf: true
hosts:
- cert_expires: Sep 10 07:09:30 2026 GMT
  host: www.betterleap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Betterleap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Betterleap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Betterleap
provider_slug: betterleap
slug: betterleap-domain-security
source_filename: betterleap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.betterleap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 07:09:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: betterleap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/betterleap/refs/heads/main/security/betterleap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Talent Acquisition
- Healthcare
- Artificial Intelligence
- Sourcing
- HR Tech
- SaaS
---
