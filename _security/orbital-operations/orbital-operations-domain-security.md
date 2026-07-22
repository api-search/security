---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: orbitalops.tech
  spf: true
hosts:
- cert_expires: Oct 13 15:21:41 2026 GMT
  host: www.orbitalops.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbital Operations Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbital Operations, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Orbital Operations
provider_slug: orbital-operations
slug: orbital-operations-domain-security
source_filename: orbital-operations-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.orbitalops.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 15:21:41 2026 GMT\n  hsts: false\ndomains:\n- domain: orbitalops.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbital-operations/refs/heads/main/security/orbital-operations-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Frontier Tech
- Space
- Space Defense
- Aerospace
- Satellite
- Orbital Systems
---
