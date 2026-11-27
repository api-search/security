---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: mindlify.co
  spf: true
hosts:
- cert_expires: Feb 15 17:15:25 2027 GMT
  host: mindlify.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mindlify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mindlify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Mindlify
provider_slug: mindlify-co
slug: mindlify-co-domain-security
source_filename: mindlify-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mindlify.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 17:15:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mindlify.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/mindlify-co/security/mindlify-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Management
- Artificial Intelligence
- Productivity
- Collaboration
- Software-as-a-Service
---
