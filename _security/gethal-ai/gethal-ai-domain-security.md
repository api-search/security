---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gethal.ai
  spf: false
hosts:
- cert_expires: Dec 21 22:43:28 2026 GMT
  host: gethal.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: GetHal.ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GetHal.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: GetHal.ai
provider_slug: gethal-ai
slug: gethal-ai-domain-security
source_filename: gethal-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gethal.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 22:43:28 2026 GMT\n  hsts: false\ndomains:\n- domain: gethal.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/gethal-ai/security/gethal-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Sales Automation
- Lead Generation
- CRM
- Dashboards
- Software-as-a-Service
---
