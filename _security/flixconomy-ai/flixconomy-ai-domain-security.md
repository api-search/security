---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: flixconomy.ai
  spf: false
hosts:
- cert_expires: Jan 19 09:59:56 2027 GMT
  host: flixconomy.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Flixconomy GmbH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flixconomy GmbH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Flixconomy GmbH
provider_slug: flixconomy-ai
slug: flixconomy-ai-domain-security
source_filename: flixconomy-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: flixconomy.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 09:59:56 2027 GMT\n  hsts: false\ndomains:\n- domain: flixconomy.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/flixconomy-ai/security/flixconomy-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Human-in-the-Loop
- MCP
- Inference
- Platform
---
