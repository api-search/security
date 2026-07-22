---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: camber.health
  spf: true
hosts:
- cert_expires: Sep 20 01:59:42 2026 GMT
  host: www.camber.health
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Juniper Behavior Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juniper Behavioral Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Juniper Behavioral Health
provider_slug: juniper-behavior-health
slug: juniper-behavior-health-domain-security
source_filename: juniper-behavior-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.camber.health\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:59:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: camber.health\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juniper-behavior-health/refs/heads/main/security/juniper-behavior-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Behavioral Health
- Healthcare
- Revenue Cycle Management
- Medical Billing
- Claims Processing
- Health Tech
- SaaS
---
