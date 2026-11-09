---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: beket.ai
  spf: true
hosts:
- cert_expires: Jan  1 14:17:01 2027 GMT
  host: beket.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Beket Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beket AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Beket AI
provider_slug: beket-ai
slug: beket-ai-domain-security
source_filename: beket-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: beket.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 14:17:01 2027 GMT\n  hsts: false\ndomains:\n- domain: beket.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/beket-ai/security/beket-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Brands
- Monitoring
- Analytics
---
