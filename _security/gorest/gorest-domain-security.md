---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: gorest.co.in
  spf: false
hosts:
- cert_expires: Aug 16 11:33:23 2026 GMT
  host: gorest.co.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gorest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gorest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: Gorest
provider_slug: gorest
slug: gorest-domain-security
source_filename: gorest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gorest.co.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:33:23 2026 GMT\n  hsts: null\ndomains:\n- domain: gorest.co.in\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorest/refs/heads/main/security/gorest-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Development
- Public APIs
---
