---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: kumbuka.ai
  spf: true
hosts:
- cert_expires: Jan 20 22:49:22 2027 GMT
  host: kumbuka.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kumbuka AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kumbuka AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Kumbuka AI
provider_slug: kumbuka-ai
slug: kumbuka-ai-domain-security
source_filename: kumbuka-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kumbuka.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 22:49:22 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kumbuka.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/kumbuka-ai/security/kumbuka-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Governance
- Memory
- Open Source
- Team Collaboration
---
