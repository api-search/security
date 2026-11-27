---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 404humans.xyz
  spf: true
hosts:
- cert_expires: Jan 23 12:36:16 2027 GMT
  host: 404humans.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 404humans.xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 404humans.xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 404humans.xyz
provider_slug: 404humans-xyz
slug: 404humans-xyz-domain-security
source_filename: 404humans-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 404humans.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 12:36:16 2027 GMT\n  hsts: false\ndomains:\n- domain: 404humans.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/404humans-xyz/security/404humans-xyz-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- On-chain Advertising
---
