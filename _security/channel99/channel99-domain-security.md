---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: channel99.com
  spf: true
hosts:
- cert_expires: Oct  2 01:27:01 2026 GMT
  host: channel99.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Channel99 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Channel99, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Channel99
provider_slug: channel99
slug: channel99-domain-security
source_filename: channel99-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channel99.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 01:27:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: channel99.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channel99/refs/heads/main/security/channel99-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Analytics
- Attribution
- B2B
- Advertising
- Marketing Technology
- Artificial Intelligence
- Account-Based Marketing
---
