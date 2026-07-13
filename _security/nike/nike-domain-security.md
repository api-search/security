---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nike.com
  spf: true
hosts:
- host: developer.nike.com
  https: false
- cert_expires: Aug  9 11:30:12 2026 GMT
  host: api.nike.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nike Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for nike, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: nike
provider_slug: nike
slug: nike-domain-security
source_filename: nike-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.nike.com\n  https: false\n- host: api.nike.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug  9 11:30:12 2026 GMT\n  hsts: null\ndomains:\n- domain: nike.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nike/refs/heads/main/security/nike-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fortune 500
---
