---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tradespace.io
  spf: true
hosts:
- cert_expires: Aug 21 22:10:40 2026 GMT
  host: tradespace.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tradespace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tradespace, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tradespace
provider_slug: tradespace
slug: tradespace-domain-security
source_filename: tradespace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tradespace.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 22:10:40 2026 GMT\n  hsts: false\ndomains:\n- domain: tradespace.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tradespace/refs/heads/main/security/tradespace-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Intellectual Property
- Patents
- IP Management
- Legal
- Legal Tech
- Licensing
- Artificial Intelligence
---
