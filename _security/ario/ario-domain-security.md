---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: heyario.com
  spf: true
hosts:
- cert_expires: Oct  1 11:55:59 2026 GMT
  host: www.heyario.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ario Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ario, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Ario
provider_slug: ario
slug: ario-domain-security
source_filename: ario-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.heyario.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 11:55:59 2026 GMT\n  hsts: null\ndomains:\n- domain: heyario.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ario/refs/heads/main/security/ario-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Ai Apps
- Artificial Intelligence
- AI
- Venture Backed
---
