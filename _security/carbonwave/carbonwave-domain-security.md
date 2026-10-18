---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: carbonwave.com
  spf: true
hosts:
- cert_expires: Jan  2 20:48:33 2027 GMT
  host: carbonwave.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Carbonwave Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carbonwave, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Carbonwave
provider_slug: carbonwave
slug: carbonwave-domain-security
source_filename: carbonwave-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: carbonwave.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 20:48:33 2027 GMT\n  hsts: false\ndomains:\n- domain: carbonwave.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carbonwave/refs/heads/main/security/carbonwave-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biomaterials
- Sustainability
- Seaweed
- Climate Tech
---
