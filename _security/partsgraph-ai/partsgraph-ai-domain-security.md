---
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: partsgraph.ai
  spf: true
hosts:
- cert_expires: Jan  7 19:47:25 2027 GMT
  host: partsgraph.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: M Heath Consulting Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for M Heath Consulting Ltd, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: M Heath Consulting Ltd
provider_slug: partsgraph-ai
slug: partsgraph-ai-domain-security
source_filename: partsgraph-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: partsgraph.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 19:47:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: partsgraph.ai\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/partsgraph-ai/security/partsgraph-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Data
- Manufacturing
- Parts
- United Kingdom
---
