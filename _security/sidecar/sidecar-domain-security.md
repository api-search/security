---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: side.cr
  spf: false
hosts:
- cert_expires: Oct 10 14:33:53 2026 GMT
  host: side.cr
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidecar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sidecar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sidecar
provider_slug: sidecar
slug: sidecar-domain-security
source_filename: sidecar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: side.cr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 14:33:53 2026 GMT\n  hsts: false\ndomains:\n- domain: side.cr\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidecar/refs/heads/main/security/sidecar-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Transportation
- Ridesharing
- Mobility
- Automotive
- News
- Content Platform
---
