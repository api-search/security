---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: elering.ee
  spf: true
hosts:
- cert_expires: Dec 23 07:06:48 2026 GMT
  host: elering.ee
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Elering Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elering, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Elering
provider_slug: elering
slug: elering-domain-security
source_filename: elering-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elering.ee\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 07:06:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: elering.ee\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/elering/security/elering-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- Transmission
- Grid
- Estonia
- Utilities
---
