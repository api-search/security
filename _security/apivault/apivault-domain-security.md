---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: apivault.dev
  spf: false
hosts:
- cert_expires: Oct  9 12:31:58 2026 GMT
  host: apivault.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apivault Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apivault, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Apivault
provider_slug: apivault
slug: apivault-domain-security
source_filename: apivault-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apivault.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 12:31:58 2026 GMT\n  hsts: false\ndomains:\n- domain: apivault.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apivault/refs/heads/main/security/apivault-domain-security.yml
summary_line: TLSv1.3
tags:
- API Catalog
- API Directory
- API Discovery
- Open Source
- Public APIs
---
