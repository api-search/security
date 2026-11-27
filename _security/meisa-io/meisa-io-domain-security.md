---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: meisa.io
  spf: true
hosts:
- cert_expires: Dec 25 22:12:43 2026 GMT
  host: meisa.io
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Meisa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Meisa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Meisa
provider_slug: meisa-io
slug: meisa-io-domain-security
source_filename: meisa-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: meisa.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 25 22:12:43 2026 GMT\n  hsts: false\ndomains:\n- domain: meisa.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/meisa-io/security/meisa-io-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Email
- Software-as-a-Service
- Onboarding
- Lifecycle
- Newsletters
---
