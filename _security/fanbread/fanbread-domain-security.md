---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: false
  dnssec: false
  domain: fanbread.com
  spf: true
hosts:
- host: fanbread.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fanbread Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fanbread, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Fanbread
provider_slug: fanbread
slug: fanbread-domain-security
source_filename: fanbread-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fanbread.com\n  https: false\ndomains:\n- domain: fanbread.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fanbread/refs/heads/main/security/fanbread-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Defunct
- Venture Backed
- 500 Global
- Media
---
