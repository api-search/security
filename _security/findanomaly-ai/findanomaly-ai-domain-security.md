---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: findanomaly.ai
  spf: true
hosts:
- cert_expires: Jan 24 16:40:41 2027 GMT
  host: findanomaly.ai
  hsts: true
  hsts_max_age: 86400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anomaly AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anomaly AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Anomaly AI
provider_slug: findanomaly-ai
slug: findanomaly-ai-domain-security
source_filename: findanomaly-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: findanomaly.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 16:40:41 2027 GMT\n  hsts: true\n  hsts_max_age: 86400\ndomains:\n- domain: findanomaly.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/findanomaly-ai/security/findanomaly-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data Analytics
- Business Intelligence
- Automation
- Software-as-a-Service
- Company
---
