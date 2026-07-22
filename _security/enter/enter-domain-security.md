---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: enter.de
  spf: true
hosts:
- cert_expires: Oct 14 05:17:26 2026 GMT
  host: www.enter.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Enter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Enter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Enter
provider_slug: enter
slug: enter-domain-security
source_filename: enter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.enter.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 05:17:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: enter.de\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enter/refs/heads/main/security/enter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Cleantech
- Energy Efficiency
- Heat Pumps
- Solar
- Building Renovation
- Germany
- Consumer
---
