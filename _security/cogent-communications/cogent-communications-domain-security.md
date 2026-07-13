---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cogentco.com
  spf: true
hosts:
- cert_expires: Sep  8 04:23:55 2026 GMT
  host: www.cogentco.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: developer.cogentco.com
  https: false
- host: api.cogentco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cogent Communications Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cogent Communications, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cogent Communications
provider_slug: cogent-communications
slug: cogent-communications-domain-security
source_filename: cogent-communications-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cogentco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 04:23:55 2026 GMT\n  hsts: false\n- host: developer.cogentco.com\n  https: false\n- host: api.cogentco.com\n  https: false\ndomains:\n- domain: cogentco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cogent-communications/refs/heads/main/security/cogent-communications-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Internet
- Network
- Data Center
---
