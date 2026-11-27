---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: eml.ai
  spf: true
hosts:
- cert_expires: Jan 25 01:25:45 2027 GMT
  host: eml.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: em[ai]l Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for em[ai]l, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: em[ai]l
provider_slug: eml-ai
slug: eml-ai-domain-security
source_filename: eml-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eml.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 01:25:45 2027 GMT\n  hsts: false\ndomains:\n- domain: eml.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/eml-ai/security/eml-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Artificial Intelligence
- Privacy
- Filtering
- Software-as-a-Service
---
