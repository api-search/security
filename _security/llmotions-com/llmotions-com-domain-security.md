---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: llmotions.com
  spf: true
hosts:
- cert_expires: Dec  1 14:01:34 2026 GMT
  host: llmotions.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llmotions Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for llmotions-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: llmotions-com
provider_slug: llmotions-com
slug: llmotions-com-domain-security
source_filename: llmotions-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llmotions.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 14:01:34 2026 GMT\n  hsts: false\ndomains:\n- domain: llmotions.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/llmotions-com/security/llmotions-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- MotionGraphics
- Animation
- Cloud
---
