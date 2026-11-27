---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lamdis.ai
  spf: true
hosts:
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: lamdis.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lamdis Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lamdis, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lamdis
provider_slug: lamdis-ai
slug: lamdis-ai-domain-security
source_filename: lamdis-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lamdis.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: lamdis.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lamdis-ai/security/lamdis-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Health
- Insurance
- Appeals
- Artificial Intelligence
- Free
---
