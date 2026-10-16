---
api_specs:
- filename: comunix-openapi-generated.yml
  format: yaml
  label: Comunix API
  slug: comunix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comunix/refs/heads/main/openapi/_ae-authored/comunix-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: getcomunix.com
  spf: false
hosts:
- cert_expires: Nov 21 02:35:46 2026 GMT
  host: www.getcomunix.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Comunix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Comunix, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Comunix
provider_slug: comunix
slug: comunix-domain-security
source_filename: comunix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getcomunix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 02:35:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: getcomunix.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comunix/refs/heads/main/security/comunix-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Gaming
- Social
- Live
- VideoChat
- Poker
---
