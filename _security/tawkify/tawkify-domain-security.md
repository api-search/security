---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tawkify.com
  spf: true
hosts:
- cert_expires: Nov  9 18:54:44 2026 GMT
  host: tawkify.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tawkify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tawkify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tawkify
provider_slug: tawkify
slug: tawkify-domain-security
source_filename: tawkify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tawkify.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 18:54:44 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tawkify.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tawkify/refs/heads/main/security/tawkify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Matchmaking
- Online Dating
- Relationships
- Consumer Services
- Personal Services
- Concierge
---
