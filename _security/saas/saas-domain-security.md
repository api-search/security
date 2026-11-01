---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: saas.industries
  spf: true
hosts:
- cert_expires: Dec 18 18:05:32 2026 GMT
  host: saas.industries
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Saas Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SaaS Industries, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: SaaS Industries
provider_slug: saas
slug: saas-domain-security
source_filename: saas-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: saas.industries\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 18:05:32 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: saas.industries\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/saas/security/saas-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- SaaS
- Platform
- API
- Integration
- Billing
---
