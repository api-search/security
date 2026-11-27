---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gigaverse.ai
  spf: true
hosts:
- cert_expires: Dec 30 14:47:10 2026 GMT
  host: gigaverse.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gigaverse AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gigaverse AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gigaverse AI
provider_slug: gigaverse-ai
slug: gigaverse-ai-domain-security
source_filename: gigaverse-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigaverse.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 14:47:10 2026 GMT\n  hsts: false\ndomains:\n- domain: gigaverse.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/gigaverse-ai/security/gigaverse-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Gig Economy
- Tax
- Retirement
- Mobile App
---
