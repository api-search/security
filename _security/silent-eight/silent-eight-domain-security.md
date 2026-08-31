---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: silenteight.com
  spf: true
hosts:
- cert_expires: Nov 22 14:05:27 2026 GMT
  host: www.silenteight.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silent Eight Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Silent Eight, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Silent Eight
provider_slug: silent-eight
slug: silent-eight-domain-security
source_filename: silent-eight-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.silenteight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 14:05:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: silenteight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silent-eight/refs/heads/main/security/silent-eight-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Crime Compliance
- Anti-Money Laundering
- Sanctions Screening
- Transaction Monitoring
- Know Your Customer
- Adverse Media
- RegTech
- Artificial Intelligence
- Agentic AI
- Financial-Services
- Compliance
---
