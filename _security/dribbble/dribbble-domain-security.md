---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dribbble.com
  spf: true
hosts:
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: developer.dribbble.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dribbble Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dribbble, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dribbble
provider_slug: dribbble
slug: dribbble-domain-security
source_filename: dribbble-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.dribbble.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: dribbble.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dribbble/refs/heads/main/security/dribbble-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Art And Design
- Public APIs
---
