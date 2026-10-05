---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: blossom-energy.co.jp
  spf: true
hosts:
- cert_expires: Nov  2 04:10:49 2026 GMT
  host: www.blossom-energy.co.jp
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blossomenergy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Blossomenergy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Blossomenergy
provider_slug: blossomenergy
slug: blossomenergy-domain-security
source_filename: blossomenergy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.blossom-energy.co.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 04:10:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: blossom-energy.co.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blossomenergy/refs/heads/main/security/blossomenergy-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Energy
- Renewables
- Startups
- Private
- Marketplace
---
