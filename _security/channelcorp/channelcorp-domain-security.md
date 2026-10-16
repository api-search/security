---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: channelcor.com
  spf: true
hosts:
- cert_expires: Nov 21 18:45:48 2026 GMT
  host: channelcor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Channelcorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Channelcorp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Channelcorp
provider_slug: channelcorp
slug: channelcorp-domain-security
source_filename: channelcorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: channelcor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 18:45:48 2026 GMT\n  hsts: false\ndomains:\n- domain: channelcor.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/channelcorp/refs/heads/main/security/channelcorp-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consulting
- Channel Economics
- Partner Finance
- AI Tools
---
