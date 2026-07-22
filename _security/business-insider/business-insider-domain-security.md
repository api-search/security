---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: businessinsider.com
  spf: true
hosts:
- cert_expires: Nov 21 06:22:55 2026 GMT
  host: www.businessinsider.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Business Insider Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Business Insider, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Business Insider
provider_slug: business-insider
slug: business-insider-domain-security
source_filename: business-insider-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.businessinsider.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 21 06:22:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: businessinsider.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/business-insider/refs/heads/main/security/business-insider-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Media
- News
- Business
- Finance
- Technology
- Publishing
---
