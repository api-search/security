---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aspect-health.com
  spf: true
hosts:
- cert_expires: Oct 15 14:16:35 2026 GMT
  host: aspect-health.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aspect Health Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aspect Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aspect Health
provider_slug: aspect-health
slug: aspect-health-domain-security
source_filename: aspect-health-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aspect-health.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aspect-health.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspect-health/refs/heads/main/security/aspect-health-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Health
- Digital Health
- Women's Health
- PCOS
- Continuous Glucose Monitoring
- Telehealth
- Nutrition
- Wellness
---
