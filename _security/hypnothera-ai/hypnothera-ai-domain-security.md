---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hypnothera.ai
  spf: true
hosts:
- cert_expires: Dec 22 15:51:09 2026 GMT
  host: hypnothera.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hypnothera Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hypnothera, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hypnothera
provider_slug: hypnothera-ai
slug: hypnothera-ai-domain-security
source_filename: hypnothera-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hypnothera.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 15:51:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hypnothera.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hypnothera-ai/security/hypnothera-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Artificial Intelligence
- Health
- Wellness
- Personalization
- Hypnosis
- Company
---
