---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: comun.app
  spf: true
hosts:
- cert_expires: Sep 17 20:09:18 2026 GMT
  host: www.comun.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Comun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comun, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Comun
provider_slug: comun
slug: comun-domain-security
source_filename: comun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.comun.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 20:09:18 2026 GMT\n  hsts: false\ndomains:\n- domain: comun.app\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comun/refs/heads/main/security/comun-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Banking
- Neobank
- Remittances
- Money Transfer
- Immigrants
- Consumer Finance
---
