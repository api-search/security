---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: d-edge.com
  spf: true
hosts:
- cert_expires: Oct 20 14:25:31 2026 GMT
  host: d-edge.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: D Edge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for D-EDGE Hospitality Solutions, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: D-EDGE Hospitality Solutions
provider_slug: d-edge
slug: d-edge-domain-security
source_filename: d-edge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: d-edge.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 14:25:31 2026 GMT\n  hsts: false\ndomains:\n- domain: d-edge.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/d-edge/refs/heads/main/security/d-edge-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- Technology
- Marketing
- Software-as-a-Service
- Company
---
