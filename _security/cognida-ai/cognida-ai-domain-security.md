---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cognida.ai
  spf: true
hosts:
- cert_expires: Jan  1 13:30:05 2027 GMT
  host: main.cognida.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cognida Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognida.ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cognida.ai
provider_slug: cognida-ai
slug: cognida-ai-domain-security
source_filename: cognida-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: main.cognida.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 13:30:05 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cognida.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognida-ai/refs/heads/main/security/cognida-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Enterprise
- Automation
- Data
- Platform
- Company
---
