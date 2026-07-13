---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kroki.io
  spf: true
hosts:
- cert_expires: Oct  2 02:56:44 2026 GMT
  host: kroki.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kroki Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kroki, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kroki
provider_slug: kroki
slug: kroki-domain-security
source_filename: kroki-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kroki.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 02:56:44 2026 GMT\n  hsts: false\ndomains:\n- domain: kroki.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kroki/refs/heads/main/security/kroki-domain-security.yml
summary_line: TLSv1.3
tags:
- Development
- Public APIs
---
