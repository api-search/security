---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: withcoverage.com
  spf: true
hosts:
- cert_expires: Aug 25 14:10:57 2026 GMT
  host: withcoverage.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Withcoverage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Withcoverage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Withcoverage
provider_slug: withcoverage
slug: withcoverage-domain-security
source_filename: withcoverage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: withcoverage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 14:10:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withcoverage.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/withcoverage/refs/heads/main/security/withcoverage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Insurtech
- Insurance
- Risk Management
- Commercial Insurance
- Brokerage
- Claims
- Fintech
---
