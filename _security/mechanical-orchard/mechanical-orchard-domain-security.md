---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: mechanical-orchard.com
  spf: true
hosts:
- cert_expires: Sep 25 13:32:32 2026 GMT
  host: www.mechanical-orchard.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mechanical Orchard Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mechanical Orchard, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mechanical Orchard
provider_slug: mechanical-orchard
slug: mechanical-orchard-domain-security
source_filename: mechanical-orchard-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mechanical-orchard.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 13:32:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mechanical-orchard.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mechanical-orchard/refs/heads/main/security/mechanical-orchard-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Mainframe Modernization
- Legacy Modernization
- Artificial Intelligence
- Cloud Migration
- Enterprise Software
- COBOL
- Government
---
