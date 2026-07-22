---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: peerless.com
  spf: true
hosts:
- cert_expires: Sep  1 20:44:10 2026 GMT
  host: www.peerless.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Peerless Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Peerless Systems, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Peerless Systems
provider_slug: peerless-systems
slug: peerless-systems-domain-security
source_filename: peerless-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.peerless.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 20:44:10 2026 GMT\n  hsts: false\ndomains:\n- domain: peerless.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peerless-systems/refs/heads/main/security/peerless-systems-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Imaging
- Embedded Systems
- Printing
- Licensing
- Technology
---
