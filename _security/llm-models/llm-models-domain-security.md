---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: llm-models.org
  spf: false
hosts:
- cert_expires: Jan  1 06:40:06 2027 GMT
  host: llm-models.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Llm Models Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AI Models Directory, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AI Models Directory
provider_slug: llm-models
slug: llm-models-domain-security
source_filename: llm-models-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: llm-models.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 06:40:06 2027 GMT\n  hsts: null\ndomains:\n- domain: llm-models.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/llm-models/refs/heads/main/security/llm-models-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
