---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: botclaw.tech
  spf: true
hosts:
- cert_expires: Dec 30 13:14:29 2026 GMT
  host: botclaw.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Botclaw Tech Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BotClaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: BotClaw
provider_slug: botclaw-tech
slug: botclaw-tech-domain-security
source_filename: botclaw-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: botclaw.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 13:14:29 2026 GMT\n  hsts: false\ndomains:\n- domain: botclaw.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/botclaw-tech/security/botclaw-tech-domain-security.yml
summary_line: TLSv1.3
tags:
- Agent Observer
- AI Agents
- Workflow Library
- Integration Guides
- Documentation
- Personal Assistants
---
