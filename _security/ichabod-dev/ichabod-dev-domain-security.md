---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ichabod.dev
  spf: false
hosts:
- cert_expires: Dec 25 08:07:54 2026 GMT
  host: ichabod.dev
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ichabod Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ichabod, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Ichabod
provider_slug: ichabod-dev
slug: ichabod-dev-domain-security
source_filename: ichabod-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ichabod.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 08:07:54 2026 GMT\n  hsts: null\ndomains:\n- domain: ichabod.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ichabod-dev/security/ichabod-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
