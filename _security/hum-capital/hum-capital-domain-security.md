---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: humcapital.com
  spf: true
hosts:
- cert_expires: Sep 29 15:46:23 2026 GMT
  host: humcapital.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hum Capital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hum Capital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hum Capital
provider_slug: hum-capital
slug: hum-capital-domain-security
source_filename: hum-capital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: humcapital.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 15:46:23 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: humcapital.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hum-capital/refs/heads/main/security/hum-capital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Capital Markets
- Fintech
- Lending
- Alternative Financing
- Investment
- Marketplace
---
