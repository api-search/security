---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: react.dev
  spf: false
hosts:
- cert_expires: Sep 13 09:57:49 2026 GMT
  host: react.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: React Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for React, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: React
provider_slug: react
slug: react-domain-security
source_filename: react-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: react.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 09:57:49 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: react.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/react/refs/heads/main/security/react-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Component-Based
- Frontend
- JavaScript
- Single Page Application
- UI Library
- Web Development
---
