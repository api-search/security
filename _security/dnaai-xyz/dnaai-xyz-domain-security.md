---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dnaai.xyz
  spf: false
hosts:
- cert_expires: Dec 23 14:08:09 2026 GMT
  host: dnaai.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DNAAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DNAAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: DNAAI
provider_slug: dnaai-xyz
slug: dnaai-xyz-domain-security
source_filename: dnaai-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dnaai.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 14:08:09 2026 GMT\n  hsts: null\ndomains:\n- domain: dnaai.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/dnaai-xyz/security/dnaai-xyz-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
