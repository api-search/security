---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pixe.la
  spf: false
hosts:
- cert_expires: Sep 24 17:03:13 2026 GMT
  host: pixe.la
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Pixela Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pixela, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Pixela
provider_slug: pixela
slug: pixela-domain-security
source_filename: pixela-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pixe.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:03:13 2026 GMT\n  hsts: false\ndomains:\n- domain: pixe.la\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pixela/refs/heads/main/security/pixela-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Tracking
- Public APIs
---
