---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: bettercomp.com
  spf: true
hosts:
- cert_expires: Dec  9 19:15:43 2026 GMT
  host: www.bettercomp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bettercomp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BetterComp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BetterComp
provider_slug: bettercomp
slug: bettercomp-domain-security
source_filename: bettercomp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bettercomp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  9 19:15:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bettercomp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bettercomp/refs/heads/main/security/bettercomp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Compensation
- HRTech
- AI
- SaaS
- Enterprise
---
