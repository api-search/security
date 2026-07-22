---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: deepstreamtech.com
  spf: true
hosts:
- cert_expires: Sep 12 06:11:47 2026 GMT
  host: deepstreamtech.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Deepstream Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DeepStream Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: DeepStream Technologies
provider_slug: deepstream-technologies
slug: deepstream-technologies-domain-security
source_filename: deepstream-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: deepstreamtech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:11:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: deepstreamtech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deepstream-technologies/refs/heads/main/security/deepstream-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Procurement
- eSourcing
- RFx
- Source-to-Contract
- Supply Chain
- Sourcing
- Contract Management
- SaaS
- AI
---
