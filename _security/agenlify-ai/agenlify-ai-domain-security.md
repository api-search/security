---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: agenlify.ai
  spf: true
hosts:
- cert_expires: Dec 26 16:37:05 2026 GMT
  host: agenlify.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agenlify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agenlify, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Agenlify
provider_slug: agenlify-ai
slug: agenlify-ai-domain-security
source_filename: agenlify-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agenlify.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 16:37:05 2026 GMT\n  hsts: false\ndomains:\n- domain: agenlify.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/agenlify-ai/security/agenlify-ai-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Directory
- Tools
- Comparison
- Agents
---
