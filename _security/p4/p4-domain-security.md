---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: p4.org
  spf: true
hosts:
- cert_expires: Sep  6 18:54:28 2026 GMT
  host: p4.org
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: P4 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for P4, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: P4
provider_slug: p4
slug: p4-domain-security
source_filename: p4-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: p4.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 18:54:28 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: p4.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/p4/refs/heads/main/security/p4-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Linux Foundation
- Networking
- Programmable
- Standards
---
