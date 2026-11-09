---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aiaam.xyz
  spf: false
hosts:
- cert_expires: Jan 13 12:25:20 2027 GMT
  host: aiaam.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aiaam Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aiaam-xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: aiaam-xyz
provider_slug: aiaam-xyz
slug: aiaam-xyz-domain-security
source_filename: aiaam-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiaam.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 12:25:20 2027 GMT\n  hsts: false\ndomains:\n- domain: aiaam.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/aiaam-xyz/security/aiaam-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Placeholder
---
