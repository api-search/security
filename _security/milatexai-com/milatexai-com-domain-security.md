---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: milatexai.com
  spf: true
hosts:
- cert_expires: Jan  2 05:40:38 2027 GMT
  host: milatexai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MiLatexAI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MiLatexAI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MiLatexAI
provider_slug: milatexai-com
slug: milatexai-com-domain-security
source_filename: milatexai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: milatexai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 05:40:38 2027 GMT\n  hsts: false\ndomains:\n- domain: milatexai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/milatexai-com/security/milatexai-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- LaTeX
- Productivity
- MCP
- Overleaf
- Version Control
---
