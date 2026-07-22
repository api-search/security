---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: american-equity.com
  spf: true
hosts:
- cert_expires: Dec 15 16:00:13 2026 GMT
  host: www.american-equity.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 01:38:36 2027 GMT
  host: register.american-equity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: American Equity Investment Life Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for American Equity Investment Life Holding, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: American Equity Investment Life Holding
provider_slug: american-equity-investment-life-holding
slug: american-equity-investment-life-holding-domain-security
source_filename: american-equity-investment-life-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.american-equity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 16:00:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: register.american-equity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 01:38:36 2027 GMT\n  hsts: false\ndomains:\n- domain: american-equity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/american-equity-investment-life-holding/refs/heads/main/security/american-equity-investment-life-holding-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial Services
- Insurance
- Annuities
- Fixed Indexed Annuity
- Retirement
- Life Insurance
- Fortune 1000
---
