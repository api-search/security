---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ibm.com
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: cloud.ibm.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Watson Natural Language Understanding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Watson Natural Language Understanding, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Watson Natural Language Understanding
provider_slug: watson-natural-language-understanding
slug: watson-natural-language-understanding-domain-security
source_filename: watson-natural-language-understanding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.ibm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: ibm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/watson-natural-language-understanding/refs/heads/main/security/watson-natural-language-understanding-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Text Analysis
- Public APIs
---
