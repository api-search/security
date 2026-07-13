---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: balldontlie.io
  spf: true
hosts:
- cert_expires: Sep  7 05:15:49 2026 GMT
  host: www.balldontlie.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Balldontlie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for balldontlie, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: balldontlie
provider_slug: balldontlie
slug: balldontlie-domain-security
source_filename: balldontlie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.balldontlie.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 05:15:49 2026 GMT\n  hsts: false\ndomains:\n- domain: balldontlie.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/balldontlie/refs/heads/main/security/balldontlie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Sports And Fitness
- Public APIs
---
