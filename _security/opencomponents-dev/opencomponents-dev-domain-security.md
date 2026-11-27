---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opencomponents.dev
  spf: true
hosts:
- cert_expires: Jan  2 12:30:31 2027 GMT
  host: opencomponents.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Open Components Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Components, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Open Components
provider_slug: opencomponents-dev
slug: opencomponents-dev-domain-security
source_filename: opencomponents-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencomponents.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 12:30:31 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opencomponents.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opencomponents-dev/security/opencomponents-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- UI Components
- User Experience
- Developer Experience
- Agentic Experience
---
