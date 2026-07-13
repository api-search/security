---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gruenstromindex.de
  spf: false
hosts:
- cert_expires: Aug 23 00:59:00 2026 GMT
  host: gruenstromindex.de
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gr Nstromindex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrünstromIndex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: GrünstromIndex
provider_slug: gr-nstromindex
slug: gr-nstromindex-domain-security
source_filename: gr-nstromindex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gruenstromindex.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 00:59:00 2026 GMT\n  hsts: false\ndomains:\n- domain: gruenstromindex.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gr-nstromindex/refs/heads/main/security/gr-nstromindex-domain-security.yml
summary_line: TLSv1.3
tags:
- Environment
- Public APIs
---
