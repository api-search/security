---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bznins.com
  spf: false
hosts:
- cert_expires: Feb  5 06:02:22 2027 GMT
  host: www.bznins.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Baozhunniu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baozhunniu, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Baozhunniu
provider_slug: baozhunniu
slug: baozhunniu-domain-security
source_filename: baozhunniu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bznins.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  5 06:02:22 2027 GMT\n  hsts: null\ndomains:\n- domain: bznins.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/baozhunniu/refs/heads/main/security/baozhunniu-domain-security.yml
summary_line: TLSv1.2
tags:
- Insurance
- Technology
- Platform
- China
- B2B
- B2C
---
