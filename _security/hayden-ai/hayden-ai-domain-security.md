---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: hayden.ai
  spf: true
hosts:
- cert_expires: Oct  8 09:55:33 2026 GMT
  host: hayden.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hayden Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hayden AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Hayden AI
provider_slug: hayden-ai
slug: hayden-ai-domain-security
source_filename: hayden-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hayden.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 09:55:33 2026 GMT\n  hsts: null\ndomains:\n- domain: hayden.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hayden-ai/refs/heads/main/security/hayden-ai-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Transportation
- Transit
- Smart Cities
- Government
- Traffic Enforcement
- Spatial Analytics
- Mobility
---
