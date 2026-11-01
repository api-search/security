---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: polymathlabs.ai
  spf: true
hosts:
- cert_expires: Dec 15 08:28:27 2026 GMT
  host: polymathlabs.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Polymathlabs Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polymath, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Polymath
provider_slug: polymathlabs-ai
slug: polymathlabs-ai-domain-security
source_filename: polymathlabs-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polymathlabs.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 08:28:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: polymathlabs.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/polymathlabs-ai/security/polymathlabs-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Simulation
- AutonomousAgents
- VentureBacked
---
