---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eidostack.com
  spf: false
hosts:
- cert_expires: Dec 31 14:51:52 2026 GMT
  host: eidostack.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eidostack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EidoStack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: EidoStack
provider_slug: eidostack
slug: eidostack-domain-security
source_filename: eidostack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eidostack.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 14:51:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eidostack.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eidostack/refs/heads/main/security/eidostack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Model Evaluation
- Platform
- SaaS
---
