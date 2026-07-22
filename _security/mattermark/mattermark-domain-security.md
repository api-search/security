---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mattermark.com
  spf: true
hosts:
- cert_expires: Sep 29 23:18:40 2026 GMT
  host: mattermark.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mattermark Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mattermark, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Mattermark
provider_slug: mattermark
slug: mattermark-domain-security
source_filename: mattermark-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mattermark.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:18:40 2026 GMT\n  hsts: false\ndomains:\n- domain: mattermark.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/security/mattermark-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Business Intelligence
- Company Data
- Investors
- Funding
- Sales Intelligence
- Market Research
---
