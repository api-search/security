---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blu.ai
  spf: true
hosts:
- cert_expires: Nov 23 15:16:24 2026 GMT
  host: blu.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Blu Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ordana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ordana
provider_slug: blu-ai
slug: blu-ai-domain-security
source_filename: blu-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blu.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 15:16:24 2026 GMT\n  hsts: false\ndomains:\n- domain: blu.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blu-ai/security/blu-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
