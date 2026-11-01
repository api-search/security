---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: liftoff.ai
  spf: true
hosts:
- cert_expires: Dec 27 21:01:47 2026 GMT
  host: liftoff.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Liftoff Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Liftoff, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Liftoff
provider_slug: liftoff-io
slug: liftoff-io-domain-security
source_filename: liftoff-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liftoff.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 21:01:47 2026 GMT\n  hsts: false\ndomains:\n- domain: liftoff.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/liftoff-io/security/liftoff-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Mobile
- Advertising
- AI
- Growth
---
