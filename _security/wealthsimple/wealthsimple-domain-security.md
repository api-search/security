---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wealthsimple.com
  spf: true
hosts:
- cert_expires: Aug 27 18:26:17 2026 GMT
  host: www.wealthsimple.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wealthsimple Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wealthsimple, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wealthsimple
provider_slug: wealthsimple
slug: wealthsimple-domain-security
source_filename: wealthsimple-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wealthsimple.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 18:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wealthsimple.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wealthsimple/refs/heads/main/security/wealthsimple-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Investing
- Wealth Management
- Cryptocurrency
- Trading
- Tax
- Banking
- Canada
---
