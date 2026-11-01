---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gohandlhealth.com
  spf: false
hosts:
- cert_expires: Dec 20 01:06:43 2026 GMT
  host: gohandlhealth.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Gohandlhealth Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Handl Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Handl Health
provider_slug: gohandlhealth-com
slug: gohandlhealth-com-domain-security
source_filename: gohandlhealth-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gohandlhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 01:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: gohandlhealth.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/gohandlhealth-com/security/gohandlhealth-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- HealthTech
- Analytics
- BenefitsConsulting
- SaaS
---
