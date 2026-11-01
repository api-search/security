---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: skybridge.tech
  spf: false
hosts:
- cert_expires: Dec 28 11:37:17 2026 GMT
  host: skybridge.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Skybridge Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for skybridge-tech, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: skybridge-tech
provider_slug: skybridge-tech
slug: skybridge-tech-domain-security
source_filename: skybridge-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skybridge.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 11:37:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: skybridge.tech\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/skybridge-tech/security/skybridge-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Framework
- OpenSource
- TypeScript
- AI
---
