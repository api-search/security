---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ownyourmind.ai
  spf: true
hosts:
- cert_expires: Jan 24 22:10:50 2027 GMT
  host: ownyourmind.ai
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Own Your Mind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Own Your Mind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Own Your Mind
provider_slug: ownyourmind-ai
slug: ownyourmind-ai-domain-security
source_filename: ownyourmind-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ownyourmind.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 22:10:50 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ownyourmind.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ownyourmind-ai/security/ownyourmind-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Decentralized AI
- Research
- Sovereignty
- Tokenomics
- Open Source
---
