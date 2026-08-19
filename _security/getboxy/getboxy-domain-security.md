---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: getboxy.co
  spf: true
hosts:
- host: www.getboxy.co
  https: false
kind: domain-security
layout: security
method: probed
name: Getboxy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Boxy (ex-Storelift), probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Boxy (ex-Storelift)
provider_slug: getboxy
slug: getboxy-domain-security
source_filename: getboxy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getboxy.co\n  https: false\ndomains:\n- domain: getboxy.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getboxy/refs/heads/main/security/getboxy-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Consumer
- Retail
- Convenience Stores
- Autonomous Stores
- Computer Vision
- France
- Defunct
---
