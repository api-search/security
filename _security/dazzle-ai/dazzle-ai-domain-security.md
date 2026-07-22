---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dazzle.ai
  spf: true
hosts:
- cert_expires: Sep 23 03:00:21 2026 GMT
  host: dazzle.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dazzle Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dazzle AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dazzle AI
provider_slug: dazzle-ai
slug: dazzle-ai-domain-security
source_filename: dazzle-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dazzle.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 03:00:21 2026 GMT\n  hsts: false\ndomains:\n- domain: dazzle.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dazzle-ai/refs/heads/main/security/dazzle-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Artificial Intelligence
- Consumer
- Pre-Launch
- Startup
---
