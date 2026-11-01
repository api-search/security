---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: vibeseo.dev
  spf: false
hosts:
- cert_expires: Dec 27 10:07:04 2026 GMT
  host: vibeseo.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vibeseo Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for vibeseo-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: vibeseo-dev
provider_slug: vibeseo-dev
slug: vibeseo-dev-domain-security
source_filename: vibeseo-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vibeseo.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 10:07:04 2026 GMT\n  hsts: false\ndomains:\n- domain: vibeseo.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/vibeseo-dev/security/vibeseo-dev-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- SEO
- Marketing
- Automation
---
