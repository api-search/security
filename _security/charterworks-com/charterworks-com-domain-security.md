---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: charterworks.com
  spf: true
hosts:
- cert_expires: Nov 15 08:41:59 2026 GMT
  host: www.charterworks.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Charterworks Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Charter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Charter
provider_slug: charterworks-com
slug: charterworks-com-domain-security
source_filename: charterworks-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.charterworks.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 08:41:59 2026 GMT\n  hsts: false\ndomains:\n- domain: charterworks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/charterworks-com/security/charterworks-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Future of Work
- AI
- Management
- Hybrid Workplace
---
