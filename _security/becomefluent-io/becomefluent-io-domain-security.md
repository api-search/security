---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: becomefluent.io
  spf: true
hosts:
- cert_expires: Jan 21 20:03:57 2027 GMT
  host: becomefluent.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fluent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fluent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Fluent
provider_slug: becomefluent-io
slug: becomefluent-io-domain-security
source_filename: becomefluent-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: becomefluent.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 20:03:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: becomefluent.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/becomefluent-io/security/becomefluent-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Productivity
- Meeting Notes
- Mobile App
- Encryption
---
