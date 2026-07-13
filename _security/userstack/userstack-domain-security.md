---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: userstack.com
  spf: true
hosts:
- cert_expires: Sep 11 20:38:42 2026 GMT
  host: userstack.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Userstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Userstack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Userstack
provider_slug: userstack
slug: userstack-domain-security
source_filename: userstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: userstack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 20:38:42 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: userstack.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/userstack/refs/heads/main/security/userstack-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Development
- Public APIs
---
