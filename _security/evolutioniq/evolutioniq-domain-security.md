---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: evolutioniq.com
  spf: true
hosts:
- cert_expires: Oct  3 02:55:55 2026 GMT
  host: evolutioniq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Evolutioniq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EvolutionIQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EvolutionIQ
provider_slug: evolutioniq
slug: evolutioniq-domain-security
source_filename: evolutioniq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: evolutioniq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:55:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: evolutioniq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolutioniq/refs/heads/main/security/evolutioniq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Insurance
- InsurTech
- Claims
- Machine Learning
- Health
---
