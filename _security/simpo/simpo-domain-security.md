---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simpo.io
  spf: true
hosts:
- host: www.simpo.io
  https: false
kind: domain-security
layout: security
method: probed
name: Simpo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simpo, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Simpo
provider_slug: simpo
slug: simpo-domain-security
source_filename: simpo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simpo.io\n  https: false\ndomains:\n- domain: simpo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpo/refs/heads/main/security/simpo-domain-security.yml
summary_line: DMARC
tags:
- Company
- Digital Adoption
- Onboarding
- User Onboarding
- In-App Guidance
- Product Adoption
- No-Code
- Customer Success
- SaaS
---
