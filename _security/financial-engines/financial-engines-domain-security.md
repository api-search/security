---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: edelmanfinancialengines.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: edelmanfinancialengines.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Financial Engines Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Financial Engines, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Financial Engines
provider_slug: financial-engines
slug: financial-engines-domain-security
source_filename: financial-engines-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: edelmanfinancialengines.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: edelmanfinancialengines.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/financial-engines/security/financial-engines-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial-Planning
- Investment-Advice
- Wealth-Management
- Retirement-Planning
- United-States
---
