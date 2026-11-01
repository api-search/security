---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: openhelm.ai
  spf: true
hosts:
- cert_expires: Dec 24 12:11:39 2026 GMT
  host: openhelm.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Openhelm Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for openhelm-ai, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: openhelm-ai
provider_slug: openhelm-ai
slug: openhelm-ai-domain-security
source_filename: openhelm-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openhelm.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 12:11:39 2026 GMT\n  hsts: false\ndomains:\n- domain: openhelm.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/openhelm-ai/security/openhelm-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Automation
- Productivity
- SaaS
- Platform
---
