---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: vinylequity.com
  spf: true
hosts:
- cert_expires: Oct 14 17:05:38 2026 GMT
  host: vinylequity.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vinyl Equity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vinyl Equity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vinyl Equity
provider_slug: vinyl-equity
slug: vinyl-equity-domain-security
source_filename: vinyl-equity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: vinylequity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 17:05:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: vinylequity.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vinyl-equity/refs/heads/main/security/vinyl-equity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Transfer Agency
- Cap Table
- Equity Management
- Shareholder Management
- Proxy & AGM
- Fintech
---
