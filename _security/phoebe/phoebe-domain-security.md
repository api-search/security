---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: withcoral.com
  spf: true
hosts:
- cert_expires: Oct  9 14:14:48 2026 GMT
  host: withcoral.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phoebe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coral, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Coral
provider_slug: phoebe
slug: phoebe-domain-security
source_filename: phoebe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withcoral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 14:14:48 2026 GMT\n  hsts: false\ndomains:\n- domain: withcoral.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phoebe/refs/heads/main/security/phoebe-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Ai
- Agents
- Model Context Protocol
- SQL
- Data Access
- Data Integration
- Developer Tools
- Open Source
---
