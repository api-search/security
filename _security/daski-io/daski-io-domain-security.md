---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: daski.io
  spf: false
hosts:
- cert_expires: Jan 12 08:09:11 2027 GMT
  host: daski.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Daski Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Daski, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Daski
provider_slug: daski-io
slug: daski-io-domain-security
source_filename: daski-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daski.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 08:09:11 2027 GMT\n  hsts: false\ndomains:\n- domain: daski.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/daski-io/security/daski-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Marketplace
- AI Agents
- Mailbox Services
- Business Formation
---
