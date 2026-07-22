---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: xtgem.com
  spf: true
hosts:
- cert_expires: Sep  7 09:28:12 2026 GMT
  host: xtgem.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Xtgem Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for XtGem, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: XtGem
provider_slug: xtgem
slug: xtgem-domain-security
source_filename: xtgem-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: xtgem.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 09:28:12 2026 GMT\n  hsts: false\ndomains:\n- domain: xtgem.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xtgem/refs/heads/main/security/xtgem-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Website Builder
- Mobile
- Hosting
- Templates
- No-Code
- Lithuania
---
