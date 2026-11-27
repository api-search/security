---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axonagentic.ai
  spf: true
hosts:
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: axonagentic.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Axon Agentic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Axon Agentic, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Axon Agentic
provider_slug: axonagentic-ai
slug: axonagentic-ai-domain-security
source_filename: axonagentic-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: axonagentic.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: axonagentic.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/axonagentic-ai/security/axonagentic-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Life Sciences
- Consulting
- Verification-first
- Multi-Agent Systems
- Biotechnology
---
