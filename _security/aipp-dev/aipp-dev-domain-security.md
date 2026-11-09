---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aipp.dev
  spf: true
hosts:
- cert_expires: Dec 29 19:04:21 2026 GMT
  host: aipp.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aipp Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIPP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: AIPP
provider_slug: aipp-dev
slug: aipp-dev-domain-security
source_filename: aipp-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aipp.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 19:04:21 2026 GMT\n  hsts: false\ndomains:\n- domain: aipp.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aipp-dev/security/aipp-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Lightning
- base-usdc
- Digital Actions
- Developer Tools
- AI Agents
---
