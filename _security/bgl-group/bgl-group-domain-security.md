---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bglgroup.com
  spf: true
hosts:
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: bglgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bgl Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BGL Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BGL Group
provider_slug: bgl-group
slug: bgl-group-domain-security
source_filename: bgl-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bglgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bglgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bgl-group/refs/heads/main/security/bgl-group-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Business Intelligence
- Consulting
- Technology Services
- Data Analytics
---
