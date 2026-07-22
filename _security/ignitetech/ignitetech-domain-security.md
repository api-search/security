---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ignitetech.com
  spf: true
hosts:
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: www.ignitetech.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ignitetech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IgniteTech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: IgniteTech
provider_slug: ignitetech
slug: ignitetech-domain-security
source_filename: ignitetech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ignitetech.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: ignitetech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ignitetech/refs/heads/main/security/ignitetech-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- SaaS
- Enterprise Software
- Artificial Intelligence
- Software Portfolio
- Customer Engagement
- Supply Chain
- Knowledge Management
---
