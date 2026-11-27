---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adplane.ai
  spf: true
hosts:
- cert_expires: Dec 15 00:01:52 2026 GMT
  host: adplane.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adplane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adplane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adplane
provider_slug: adplane-ai
slug: adplane-ai-domain-security
source_filename: adplane-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adplane.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 00:01:52 2026 GMT\n  hsts: false\ndomains:\n- domain: adplane.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adplane-ai/security/adplane-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Ads
- Artificial Intelligence
- ChatGPT
- Claude
- Marketing Automation
- Ad Management
---
