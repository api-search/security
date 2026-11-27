---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: thesisloop.ai
  spf: true
hosts:
- cert_expires: Jan 21 08:34:40 2027 GMT
  host: thesisloop.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ThesisLoop Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ThesisLoop, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ThesisLoop
provider_slug: thesisloop-ai
slug: thesisloop-ai-domain-security
source_filename: thesisloop-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thesisloop.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 08:34:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: thesisloop.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/thesisloop-ai/security/thesisloop-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Investment Research
- US Equities
- Institutional Research
- Macro Scenarios
- Agentic Trading
---
