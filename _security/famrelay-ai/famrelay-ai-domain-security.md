---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: famrelay.ai
  spf: true
hosts:
- cert_expires: Jan  4 11:23:54 2027 GMT
  host: famrelay.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FamRelay Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FamRelay, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FamRelay
provider_slug: famrelay-ai
slug: famrelay-ai-domain-security
source_filename: famrelay-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: famrelay.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 11:23:54 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: famrelay.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/famrelay-ai/security/famrelay-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Family
- Collaboration
- Privacy
- Relay
---
