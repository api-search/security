---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: meetdavis.com
  spf: false
hosts:
- cert_expires: Oct  1 15:18:01 2026 GMT
  host: www.meetdavis.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Meetdavis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for meetdavis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: meetdavis
provider_slug: meetdavis
slug: meetdavis-domain-security
source_filename: meetdavis-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.meetdavis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 15:18:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: meetdavis.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/meetdavis/refs/heads/main/security/meetdavis-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Real Estate
- Artificial Intelligence
- PropTech
- Architecture
- Construction
- Feasibility Studies
---
