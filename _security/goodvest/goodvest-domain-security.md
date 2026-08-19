---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: goodvest.fr
  spf: true
hosts:
- cert_expires: Nov 12 07:38:47 2026 GMT
  host: www.goodvest.fr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Goodvest Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Goodvest, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Goodvest
provider_slug: goodvest
slug: goodvest-domain-security
source_filename: goodvest-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.goodvest.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 07:38:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: goodvest.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goodvest/refs/heads/main/security/goodvest-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Climate Tech
- Fintech
- Financial Services
- Investing
- Wealth Management
- Sustainable Finance
- ESG
- Insurance
- Retirement
- France
---
