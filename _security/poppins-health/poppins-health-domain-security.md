---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: poppinshealth.com
  spf: true
hosts:
- host: www.poppinshealth.com
  https: false
kind: domain-security
layout: security
method: probed
name: Poppins Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Poppins Health, probed live across 1 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Poppins Health
provider_slug: poppins-health
slug: poppins-health-domain-security
source_filename: poppins-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.poppinshealth.com\n  https: false\ndomains:\n- domain: poppinshealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/poppins-health/refs/heads/main/security/poppins-health-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Health Insurance
- Insurance
- Healthcare
- Small Business
- Employee Benefits
- Insurtech
---
