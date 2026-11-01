---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: zenith-ai.one
  spf: true
hosts:
- cert_expires: Dec 12 22:54:42 2026 GMT
  host: zenith-ai.one
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zenith Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zenith-AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Zenith-AI
provider_slug: zenith-ai
slug: zenith-ai-domain-security
source_filename: zenith-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zenith-ai.one\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 22:54:42 2026 GMT\n  hsts: null\ndomains:\n- domain: zenith-ai.one\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/zenith-ai/security/zenith-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Enterprise
- Automation
---
