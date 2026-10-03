---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baconwork.com
  spf: true
hosts:
- cert_expires: Dec 13 06:18:13 2026 GMT
  host: www.baconwork.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bacon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bacon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bacon
provider_slug: bacon
slug: bacon-domain-security
source_filename: bacon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.baconwork.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 06:18:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: baconwork.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bacon/refs/heads/main/security/bacon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- GigWork
- Staffing
- On-Demand
- Marketplace
- Utah
---
