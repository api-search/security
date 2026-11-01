---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tryscope.com
  spf: false
hosts:
- cert_expires: Jan 12 17:05:39 2027 GMT
  host: tryscope.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Tryscope Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scope, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Scope
provider_slug: tryscope-com
slug: tryscope-com-domain-security
source_filename: tryscope-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tryscope.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 17:05:39 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tryscope.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/tryscope-com/security/tryscope-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Analytics
- Platform
- Marketing
---
