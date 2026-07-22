---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cognuse.com
  spf: true
hosts:
- host: cognuse.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cognuse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cognuse, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Cognuse
provider_slug: cognuse
slug: cognuse-domain-security
source_filename: cognuse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cognuse.com\n  https: false\ndomains:\n- domain: cognuse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cognuse/refs/heads/main/security/cognuse-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Healthcare
- Digital Health
- Rehabilitation
- Patient Engagement
- Care Continuum
- Clinical Guidelines
- Chronic Disease Management
---
