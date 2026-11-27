---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ignission.io
  spf: true
hosts:
- cert_expires: May 21 14:41:28 2027 GMT
  host: ignission.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ignission Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ignission, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ignission
provider_slug: ignission-io
slug: ignission-io-domain-security
source_filename: ignission-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ignission.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May 21 14:41:28 2027 GMT\n  hsts: false\ndomains:\n- domain: ignission.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ignission-io/security/ignission-io-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- TikTok
- Content
- Creators
- Platform
---
