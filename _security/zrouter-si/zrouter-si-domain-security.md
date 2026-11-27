---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zrouter.si
  spf: true
hosts:
- cert_expires: Jan  4 06:09:04 2027 GMT
  host: zrouter.si
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: zrouter-si Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for zrouter-si, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: zrouter-si
provider_slug: zrouter-si
slug: zrouter-si-domain-security
source_filename: zrouter-si-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zrouter.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 06:09:04 2027 GMT\n  hsts: null\ndomains:\n- domain: zrouter.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zrouter-si/security/zrouter-si-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- API Gateway
- OpenAI-Compatible
- Multi-Model
---
