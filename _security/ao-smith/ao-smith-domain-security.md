---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aosmith.com
  spf: true
hosts:
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: www.aosmith.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- host: api.aosmith.com
  https: false
kind: domain-security
layout: security
method: probed
name: Ao Smith Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AO Smith, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AO Smith
provider_slug: ao-smith
slug: ao-smith-domain-security
source_filename: ao-smith-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aosmith.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.aosmith.com\n  https: false\ndomains:\n- domain: aosmith.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ao-smith/refs/heads/main/security/ao-smith-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- IoT
- Manufacturing
- Smart Home
- Water Heaters
---
