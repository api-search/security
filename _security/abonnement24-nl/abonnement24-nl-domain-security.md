---
api_specs:
- filename: abonnement24-nl-mcp.json
  format: json
  label: Abonnement24 API
  slug: abonnement24-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/abonnement24-nl/openapi/abonnement24-nl-mcp.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: abonnement24.nl
  spf: false
hosts:
- cert_expires: Jan 14 15:38:26 2027 GMT
  host: abonnement24.nl
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Abonnement24 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abonnement24, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=reject).'
provider_name: Abonnement24
provider_slug: abonnement24-nl
slug: abonnement24-nl-domain-security
source_filename: abonnement24-nl-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abonnement24.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 15:38:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: abonnement24.nl\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/abonnement24-nl/security/abonnement24-nl-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Telecommunications
- Comparison
- Netherlands
- Mobile
- Internet
---
