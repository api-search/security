---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: caddi.com
  spf: true
hosts:
- cert_expires: Sep 10 01:43:42 2026 GMT
  host: caddi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Caddi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CADDi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CADDi
provider_slug: caddi
slug: caddi-domain-security
source_filename: caddi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: caddi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 01:43:42 2026 GMT\n  hsts: false\ndomains:\n- domain: caddi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caddi/refs/heads/main/security/caddi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Industrial
- Manufacturing
- Procurement
- Supply Chain
- Engineering Data
- Artificial Intelligence
---
