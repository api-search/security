---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ooda-health.com
  spf: true
hosts:
- cert_expires: Aug 29 22:39:17 2026 GMT
  host: ooda-health.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ooda Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ooda Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Ooda Health
provider_slug: ooda-health
slug: ooda-health-domain-security
source_filename: ooda-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ooda-health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 22:39:17 2026 GMT\n  hsts: false\ndomains:\n- domain: ooda-health.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ooda-health/refs/heads/main/security/ooda-health-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Healthcare
- Payments
- Health Insurance
- Medical Billing
- Revenue Cycle Management
- Fintech
---
