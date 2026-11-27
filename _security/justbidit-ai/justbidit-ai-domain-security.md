---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: justbidit.ai
  spf: true
hosts:
- cert_expires: Jan 12 09:01:40 2027 GMT
  host: justbidit.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bidit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bidit, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Bidit
provider_slug: justbidit-ai
slug: justbidit-ai-domain-security
source_filename: justbidit-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: justbidit.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 09:01:40 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: justbidit.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/justbidit-ai/security/justbidit-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketplace
- ReverseAuction
- Services
- Artificial Intelligence
- Consumer
---
