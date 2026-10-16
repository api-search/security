---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: cellcontrolbio.com
  spf: true
hosts:
- cert_expires: Dec 15 09:53:47 2026 GMT
  host: cellcontrolbio.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cellcontrol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cellcontrol, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Cellcontrol
provider_slug: cellcontrol
slug: cellcontrol-domain-security
source_filename: cellcontrol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cellcontrolbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 09:53:47 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: cellcontrolbio.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellcontrol/refs/heads/main/security/cellcontrol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Biotechnology
- Cell Therapy
- CAR-T
- Therapeutics
- Company
---
