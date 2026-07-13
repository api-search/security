---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: speclynx.com
  spf: true
hosts:
- cert_expires: Aug 12 08:53:23 2026 GMT
  host: speclynx.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Speclynx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SpecLynx, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: SpecLynx
provider_slug: speclynx
slug: speclynx-domain-security
source_filename: speclynx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: speclynx.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 08:53:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: speclynx.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/speclynx/refs/heads/main/security/speclynx-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Design
- AsyncAPI
- Developer Tools
- JSON Schema
- OpenAPI
- Toolkit
- VSCode
---
