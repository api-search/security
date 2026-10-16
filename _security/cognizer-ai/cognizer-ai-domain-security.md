---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cognizer.ai
  spf: true
hosts:
- cert_expires: Dec 12 16:32:25 2026 GMT
  host: cognizer.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cognizer Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognizer AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cognizer AI
provider_slug: cognizer-ai
slug: cognizer-ai-domain-security
source_filename: cognizer-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognizer.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 16:32:25 2026 GMT\n  hsts: false\ndomains:\n- domain: cognizer.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognizer-ai/refs/heads/main/security/cognizer-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Contract Intelligence
- SaaS
- LegalTech
---
