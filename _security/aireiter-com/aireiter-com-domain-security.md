---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: aireiter.com
  spf: true
hosts:
- cert_expires: Dec 31 03:49:48 2026 GMT
  host: aireiter.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aireiter Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIReiter, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AIReiter
provider_slug: aireiter-com
slug: aireiter-com-domain-security
source_filename: aireiter-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aireiter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 03:49:48 2026 GMT\n  hsts: false\ndomains:\n- domain: aireiter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aireiter-com/security/aireiter-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Multimodal
- Generation
- OpenAI-Compatible
- Credit-Pricing
---
