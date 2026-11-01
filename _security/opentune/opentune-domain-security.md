---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: weboasis.io
  spf: true
hosts:
- cert_expires: Dec 31 05:27:38 2026 GMT
  host: weboasis.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Opentune Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weboasis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Weboasis
provider_slug: opentune
slug: opentune-domain-security
source_filename: opentune-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weboasis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 05:27:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weboasis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/opentune/security/opentune-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Web3
- Artificial Intelligence
- Software-as-a-Service
- Platform
---
