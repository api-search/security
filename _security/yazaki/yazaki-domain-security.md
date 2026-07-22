---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: yazaki-group.com
  spf: true
hosts:
- cert_expires: Dec  5 23:59:59 2026 GMT
  host: www.yazaki-group.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yazaki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yazaki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Yazaki
provider_slug: yazaki
slug: yazaki-domain-security
source_filename: yazaki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yazaki-group.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: yazaki-group.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yazaki/refs/heads/main/security/yazaki-domain-security.yml
summary_line: TLSv1.3
tags:
- Automotive
- Tier 1 Supplier
- Wiring Harnesses
- Connectors
- Instrumentation
---
