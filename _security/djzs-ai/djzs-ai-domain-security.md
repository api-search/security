---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: djzs.ai
  spf: true
hosts:
- cert_expires: Jan  1 01:13:47 2027 GMT
  host: djzs.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Djzs Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DJZS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DJZS
provider_slug: djzs-ai
slug: djzs-ai-domain-security
source_filename: djzs-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: djzs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 01:13:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: djzs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/djzs-ai/security/djzs-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Trading
- Auditing
- Autonomous Agents
- Finance
---
