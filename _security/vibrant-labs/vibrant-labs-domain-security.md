---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: vibrantlabs.com
  spf: false
hosts:
- cert_expires: Jan  2 05:39:28 2027 GMT
  host: vibrantlabs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Vibrant Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vibrant Labs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Vibrant Labs
provider_slug: vibrant-labs
slug: vibrant-labs-domain-security
source_filename: vibrant-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vibrantlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 05:39:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vibrantlabs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/vibrant-labs/security/vibrant-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- AI
- Research
- OpenSource
- DataHarvesting
---
