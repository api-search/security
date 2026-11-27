---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finstat.ai
  spf: true
hosts:
- cert_expires: Jan 27 08:31:24 2027 GMT
  host: finstat.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: FinStat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinStat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FinStat
provider_slug: finstat-ai
slug: finstat-ai-domain-security
source_filename: finstat-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: finstat.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 08:31:24 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: finstat.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/finstat-ai/security/finstat-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Accounting
- Artificial Intelligence
- Integration
- Software-as-a-Service
- Company
---
