---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: adept.ai
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: huggingface.co
  spf: true
hosts:
- cert_expires: Sep 23 14:18:01 2026 GMT
  host: www.adept.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 23:59:59 2026 GMT
  host: huggingface.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Adept Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adept, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Adept
provider_slug: adept
slug: adept-domain-security
source_filename: adept-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.adept.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 14:18:01 2026 GMT\n  hsts: null\n- host: huggingface.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: adept.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: huggingface.co\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adept/refs/heads/main/security/adept-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- AI
- Agents
- Foundation Models
- Action Models
- Workflow Automation
- Multimodal
---
