---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: 01a.com
  spf: true
hosts:
- cert_expires: Sep  4 21:21:20 2026 GMT
  host: 01a.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 01 Advisors Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 01 Advisors, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: 01 Advisors
provider_slug: 01-advisors
slug: 01-advisors-domain-security
source_filename: 01-advisors-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 01a.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 21:21:20 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: 01a.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/01-advisors/refs/heads/main/security/01-advisors-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Venture Capital
- Venture Firm
- Investor
- Startups
- Series B
- San Francisco
- New York
- Advisory
---
