---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: facet.com
  spf: true
hosts:
- cert_expires: Sep 14 15:56:25 2026 GMT
  host: facet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Facet Wealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Facet Wealth, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Facet Wealth
provider_slug: facet-wealth
slug: facet-wealth-domain-security
source_filename: facet-wealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: facet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 15:56:25 2026 GMT\n  hsts: false\ndomains:\n- domain: facet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/facet-wealth/refs/heads/main/security/facet-wealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Financial Services
- Financial Planning
- Wealth Management
- Investment Management
- Retirement Planning
- Tax Planning
- Registered Investment Advisor
- Personal Finance
---
