---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: withsable.com
  spf: true
hosts:
- cert_expires: Jan 24 03:31:06 2027 GMT
  host: withsable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sable Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sable AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sable AI
provider_slug: sable-ai
slug: sable-ai-domain-security
source_filename: sable-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withsable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 03:31:06 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: withsable.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sable-ai/security/sable-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Product-Demos
- Sales-Automation
- Enterprise
---
