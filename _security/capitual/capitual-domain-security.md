---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: capitual.com
  spf: true
hosts:
- cert_expires: Dec 20 09:18:23 2026 GMT
  host: capitual.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capitual Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capitual, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Capitual
provider_slug: capitual
slug: capitual-domain-security
source_filename: capitual-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: capitual.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 09:18:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: capitual.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitual/refs/heads/main/security/capitual-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
