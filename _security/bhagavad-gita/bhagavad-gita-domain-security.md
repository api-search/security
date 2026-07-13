---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bhagavadgitaapi.in
  spf: true
hosts:
- cert_expires: Oct  4 22:11:26 2026 GMT
  host: docs.bhagavadgitaapi.in
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bhagavad Gita Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bhagavad Gita, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bhagavad Gita
provider_slug: bhagavad-gita
slug: bhagavad-gita-domain-security
source_filename: bhagavad-gita-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.bhagavadgitaapi.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 22:11:26 2026 GMT\n  hsts: false\ndomains:\n- domain: bhagavadgitaapi.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bhagavad-gita/refs/heads/main/security/bhagavad-gita-domain-security.yml
summary_line: TLSv1.3
tags:
- Books
- Public APIs
---
