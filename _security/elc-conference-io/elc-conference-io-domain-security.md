---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elc-conference.io
  spf: true
hosts:
- cert_expires: Dec 26 20:31:08 2026 GMT
  host: elc-conference.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Engineering Leadership Conference Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Engineering Leadership Conference, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Engineering Leadership Conference
provider_slug: elc-conference-io
slug: elc-conference-io-domain-security
source_filename: elc-conference-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: elc-conference.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 20:31:08 2026 GMT\n  hsts: false\ndomains:\n- domain: elc-conference.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/elc-conference-io/security/elc-conference-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Conferences
- Engineering
- Leadership
- Prague
- '2027'
- Technology
---
