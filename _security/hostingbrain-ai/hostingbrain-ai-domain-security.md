---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hostingbrain.ai
  spf: true
hosts:
- cert_expires: Jan  2 14:56:56 2027 GMT
  host: hostingbrain.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: HostingBrain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HostingBrain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HostingBrain
provider_slug: hostingbrain-ai
slug: hostingbrain-ai-domain-security
source_filename: hostingbrain-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hostingbrain.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 14:56:56 2027 GMT\n  hsts: false\ndomains:\n- domain: hostingbrain.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hostingbrain-ai/security/hostingbrain-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hosting
- Market Intelligence
- European
- Data
- Research
---
