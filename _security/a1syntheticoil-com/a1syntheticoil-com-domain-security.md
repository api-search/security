---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: a1syntheticoil.com
  spf: true
hosts:
- cert_expires: Dec 13 07:56:49 2026 GMT
  host: a1syntheticoil.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: A1 Synthetic Oil Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for A1 Synthetic Oil, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: A1 Synthetic Oil
provider_slug: a1syntheticoil-com
slug: a1syntheticoil-com-domain-security
source_filename: a1syntheticoil-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: a1syntheticoil.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 07:56:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: a1syntheticoil.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/a1syntheticoil-com/security/a1syntheticoil-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Oil
- Automotive
- Dealers
- Synthetic
- AMSOIL
- Washington
---
