---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: perfios.com
  spf: true
hosts:
- cert_expires: Aug 30 23:59:59 2026 GMT
  host: www.perfios.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Perfios Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Perfios, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Perfios
provider_slug: perfios
slug: perfios-domain-security
source_filename: perfios-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.perfios.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: perfios.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/perfios/refs/heads/main/security/perfios-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Financial Services
- KYC
- Onboarding
- Credit Decisioning
- Bank Statement Analysis
- Fraud Detection
- Account Aggregator
- India
---
