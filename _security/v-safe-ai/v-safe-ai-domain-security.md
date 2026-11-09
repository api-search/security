---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: v-safe.ai
  spf: false
hosts:
- cert_expires: Jan 12 16:31:25 2027 GMT
  host: v-safe.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: V Safe Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for v-safe-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: v-safe-ai
provider_slug: v-safe-ai
slug: v-safe-ai-domain-security
source_filename: v-safe-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: v-safe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 16:31:25 2027 GMT\n  hsts: false\ndomains:\n- domain: v-safe.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/v-safe-ai/security/v-safe-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Risk Management
- Compliance
- Israeli
- Artificial Intelligence
---
