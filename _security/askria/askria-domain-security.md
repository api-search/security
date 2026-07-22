---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: askria.ai
  spf: false
hosts:
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: askria.ai
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Askria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Askria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Askria
provider_slug: askria
slug: askria-domain-security
source_filename: askria-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: askria.ai\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: askria.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/askria/refs/heads/main/security/askria-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Venture Capital
- Private Capital
- Due Diligence
- Deal Management
- Artificial Intelligence
- Investment
- Fintech
---
