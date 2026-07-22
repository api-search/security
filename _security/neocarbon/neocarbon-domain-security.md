---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: neocarbon.tech
  spf: true
hosts:
- cert_expires: Jan 28 23:59:59 2027 GMT
  host: www.neocarbon.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Neocarbon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Neocarbon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Neocarbon
provider_slug: neocarbon
slug: neocarbon-domain-security
source_filename: neocarbon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.neocarbon.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: neocarbon.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neocarbon/refs/heads/main/security/neocarbon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Climate Tech
- Carbon Capture
- Data Centers
- Cooling
- Sustainability
- Waste Heat Recovery
- Berlin
---
