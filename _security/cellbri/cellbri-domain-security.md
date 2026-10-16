---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cellbri.com
  spf: false
hosts:
- cert_expires: Dec 14 00:04:03 2026 GMT
  host: cellbri.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellbri Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellbri, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Cellbri
provider_slug: cellbri
slug: cellbri-domain-security
source_filename: cellbri-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cellbri.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 00:04:03 2026 GMT\n  hsts: false\ndomains:\n- domain: cellbri.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellbri/refs/heads/main/security/cellbri-domain-security.yml
summary_line: TLSv1.3
tags:
- Biotechnology
- Cell Therapy
- Automation
- Manufacturing
- Platform
- Company
---
