---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: truktop.com
  spf: true
hosts:
- cert_expires: Aug 31 14:32:55 2026 GMT
  host: truktop.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automotop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automotop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Automotop
provider_slug: automotop
slug: automotop-domain-security
source_filename: automotop-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: truktop.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 14:32:55 2026 GMT\n  hsts: null\ndomains:\n- domain: truktop.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automotop/refs/heads/main/security/automotop-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
