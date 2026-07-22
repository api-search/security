---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kinro.com
  spf: true
hosts:
- cert_expires: Aug 25 20:45:27 2026 GMT
  host: www.kinro.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kinro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kinro, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kinro
provider_slug: kinro
slug: kinro-domain-security
source_filename: kinro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kinro.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 20:45:27 2026 GMT\n  hsts: false\ndomains:\n- domain: kinro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kinro/refs/heads/main/security/kinro-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- InsurTech
- Artificial Intelligence
- Small Business
- Commercial Insurance
- Brokerage
- Automation
- Y Combinator
---
