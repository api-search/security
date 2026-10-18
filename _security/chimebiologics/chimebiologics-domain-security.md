---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: chimebiologics.com
  spf: true
hosts:
- cert_expires: Jan  2 02:42:16 2027 GMT
  host: chimebiologics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Chimebiologics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chimebiologics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Chimebiologics
provider_slug: chimebiologics
slug: chimebiologics-domain-security
source_filename: chimebiologics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chimebiologics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 02:42:16 2027 GMT\n  hsts: false\ndomains:\n- domain: chimebiologics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chimebiologics/refs/heads/main/security/chimebiologics-domain-security.yml
summary_line: TLSv1.3
tags:
- CDMO
- Biologics
- Cell Line Development
- Process Development
- Protein Science
- Technology-Transfer
---
