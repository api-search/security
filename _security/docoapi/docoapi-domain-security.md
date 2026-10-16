---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: docoapi.com
  spf: true
hosts:
- cert_expires: Dec 25 19:06:02 2026 GMT
  host: docoapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docoapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Saga Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Saga Labs
provider_slug: docoapi
slug: docoapi-domain-security
source_filename: docoapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docoapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 19:06:02 2026 GMT\n  hsts: false\ndomains:\n- domain: docoapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docoapi/refs/heads/main/security/docoapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- API Documentation
- Developer Tools
- SaaS
- FastAPI
---
