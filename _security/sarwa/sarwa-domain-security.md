---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sarwa.co
  spf: true
hosts:
- cert_expires: Sep 30 12:56:11 2026 GMT
  host: sarwa.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sarwa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sarwa, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sarwa
provider_slug: sarwa
slug: sarwa-domain-security
source_filename: sarwa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sarwa.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:56:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: sarwa.co\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sarwa/refs/heads/main/security/sarwa-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- FinTech
- Investing
- Wealth Management
- Robo-Advisor
- Stock Trading
- Savings
- UAE
- ADGM
---
