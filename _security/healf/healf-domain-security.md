---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: healf.mx
  spf: true
hosts:
- cert_expires: Aug  1 04:13:20 2026 GMT
  host: healf.mx
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Healf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Healf, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Healf
provider_slug: healf
slug: healf-domain-security
source_filename: healf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: healf.mx\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  1 04:13:20 2026 GMT\n  hsts: false\ndomains:\n- domain: healf.mx\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/healf/refs/heads/main/security/healf-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- InsurTech
- Insurance
- Health Insurance
- Artificial Intelligence
- SaaS
- Mexico
- Brokers
---
