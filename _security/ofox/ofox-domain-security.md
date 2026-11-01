---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ofox.ai
  spf: true
hosts:
- cert_expires: Jan 14 14:11:45 2027 GMT
  host: ofox.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ofox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NICE TALK, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: NICE TALK
provider_slug: ofox
slug: ofox-domain-security
source_filename: ofox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ofox.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 14:11:45 2027 GMT\n  hsts: false\ndomains:\n- domain: ofox.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ofox/security/ofox-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- Platform
---
