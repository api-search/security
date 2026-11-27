---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: authoryze.ai
  spf: true
hosts:
- cert_expires: Jan 28 16:36:24 2027 GMT
  host: authoryze.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Authoryze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Authoryze, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Authoryze
provider_slug: authoryze-ai
slug: authoryze-ai-domain-security
source_filename: authoryze-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: authoryze.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 28 16:36:24 2027 GMT\n  hsts: null\ndomains:\n- domain: authoryze.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/authoryze-ai/security/authoryze-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Fintech
- Payments
- Artificial Intelligence
- Security
- Platform
---
