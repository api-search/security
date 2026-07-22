---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: markerly.com
  spf: true
hosts:
- cert_expires: Sep  5 03:18:13 2026 GMT
  host: markerly.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Markerly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Markerly, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Markerly
provider_slug: markerly
slug: markerly-domain-security
source_filename: markerly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: markerly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 03:18:13 2026 GMT\n  hsts: false\ndomains:\n- domain: markerly.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/markerly/refs/heads/main/security/markerly-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Influencer Marketing
- Marketing
- Creator Economy
- Advertising
- Social Media
- Advocacy
---
