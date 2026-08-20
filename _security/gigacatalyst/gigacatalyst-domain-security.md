---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gigacatalyst.com
  spf: true
hosts:
- cert_expires: Oct 24 13:56:15 2026 GMT
  host: gigacatalyst.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 16:58:01 2026 GMT
  host: v2.gigacatalyst.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gigacatalyst Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gigacatalyst, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gigacatalyst
provider_slug: gigacatalyst
slug: gigacatalyst-domain-security
source_filename: gigacatalyst-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gigacatalyst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 13:56:15 2026 GMT\n  hsts: false\n- host: v2.gigacatalyst.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 16:58:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gigacatalyst.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gigacatalyst/refs/heads/main/security/gigacatalyst-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Software-as-a-Service
- Sales Enablement
- Solutions Engineering
- Customer Success
- Automation
- No-Code
- Agents
- Embedded Analytics
- Low-Code
- Developer Tools
- Y Combinator
---
