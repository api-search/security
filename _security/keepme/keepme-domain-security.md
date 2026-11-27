---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: keepme.ai
  spf: true
hosts:
- cert_expires: Jan 31 02:25:07 2027 GMT
  host: keepme.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keepme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keepme, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Keepme
provider_slug: keepme
slug: keepme-domain-security
source_filename: keepme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: keepme.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 02:25:07 2027 GMT\n  hsts: false\ndomains:\n- domain: keepme.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/keepme/security/keepme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Fitness
- Software-as-a-Service
- Automation
---
