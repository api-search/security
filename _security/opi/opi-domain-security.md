---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opiproject.org
  spf: false
hosts:
- cert_expires: Aug 27 19:15:50 2026 GMT
  host: opiproject.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Programmable Infrastructure, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Open Programmable Infrastructure
provider_slug: opi
slug: opi-domain-security
source_filename: opi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opiproject.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 19:15:50 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: opiproject.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opi/refs/heads/main/security/opi-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- DPU
- Infrastructure
- Linux Foundation
- Networking
---
