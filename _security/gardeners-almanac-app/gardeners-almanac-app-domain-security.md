---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gardeners-almanac.app
  spf: true
hosts:
- cert_expires: Dec 18 18:57:41 2026 GMT
  host: gardeners-almanac.app
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gardener's Almanac Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gardener''s Almanac, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gardener's Almanac
provider_slug: gardeners-almanac-app
slug: gardeners-almanac-app-domain-security
source_filename: gardeners-almanac-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gardeners-almanac.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 18:57:41 2026 GMT\n  hsts: false\ndomains:\n- domain: gardeners-almanac.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/gardeners-almanac-app/security/gardeners-almanac-app-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
