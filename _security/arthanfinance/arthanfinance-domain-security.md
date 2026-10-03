---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: arthan.finance
  spf: true
hosts:
- cert_expires: Nov 22 03:27:48 2026 GMT
  host: arthan.finance
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Arthanfinance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Arthanfinance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Arthanfinance
provider_slug: arthanfinance
slug: arthanfinance-domain-security
source_filename: arthanfinance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: arthan.finance\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 22 03:27:48 2026 GMT\n  hsts: false\ndomains:\n- domain: arthan.finance\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arthanfinance/refs/heads/main/security/arthanfinance-domain-security.yml
summary_line: TLSv1.2 · DNSSEC · DMARC
tags:
- Company
- Fintech
- Loans
- Small Business
- India
---
