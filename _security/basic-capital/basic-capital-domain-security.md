---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: basiccapital.com
  spf: true
hosts:
- cert_expires: Aug 23 03:13:17 2026 GMT
  host: basiccapital.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Basic Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Basic Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Basic Capital
provider_slug: basic-capital
slug: basic-capital-domain-security
source_filename: basic-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: basiccapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 03:13:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: basiccapital.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basic-capital/refs/heads/main/security/basic-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Retirement
- 401k
- Investing
- Wealth Management
- Financial Services
---
