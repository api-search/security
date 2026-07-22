---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: endowus.com
  spf: true
hosts:
- cert_expires: Jan  6 23:59:59 2027 GMT
  host: endowus.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Endowus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Endowus, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Endowus
provider_slug: endowus
slug: endowus-domain-security
source_filename: endowus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: endowus.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: endowus.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/endowus/refs/heads/main/security/endowus-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wealth Management
- Fintech
- Investing
- Robo-Advisor
- Financial Services
- Singapore
- Hong Kong
---
