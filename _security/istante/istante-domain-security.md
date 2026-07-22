---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: istante.ai
  spf: false
hosts:
- cert_expires: Sep 10 12:03:04 2026 GMT
  host: istante.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Istante Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Istante, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Istante
provider_slug: istante
slug: istante-domain-security
source_filename: istante-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: istante.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:03:04 2026 GMT\n  hsts: false\ndomains:\n- domain: istante.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istante/refs/heads/main/security/istante-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Artificial Intelligence
- AI Agents
- Business Process Automation
- Automation
- Compliance
- Italy
---
