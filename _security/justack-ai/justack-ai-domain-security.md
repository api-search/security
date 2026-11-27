---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: justack.ai
  spf: true
hosts:
- cert_expires: Feb  8 14:38:48 2027 GMT
  host: justack.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Justack.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Justack.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Justack.ai
provider_slug: justack-ai
slug: justack-ai-domain-security
source_filename: justack-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justack.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  8 14:38:48 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: justack.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/justack-ai/security/justack-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Open Source
- Canada
- Access to Justice
- Non-Profit
---
