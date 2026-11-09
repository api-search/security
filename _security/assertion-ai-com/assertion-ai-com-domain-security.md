---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: assertion-ai.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: assertion-ai.com
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Assertion Ai Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assertion AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Assertion AI
provider_slug: assertion-ai-com
slug: assertion-ai-com-domain-security
source_filename: assertion-ai-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: assertion-ai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: assertion-ai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/assertion-ai-com/security/assertion-ai-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Memory
- Collaboration
- LLM
- Productivity
---
