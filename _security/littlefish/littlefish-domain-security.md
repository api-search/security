---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: littlefishapp.com
  spf: true
hosts:
- cert_expires: Sep 30 16:58:52 2026 GMT
  host: littlefishapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Littlefish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for littlefish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: littlefish
provider_slug: littlefish
slug: littlefish-domain-security
source_filename: littlefish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: littlefishapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 16:58:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: littlefishapp.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/littlefish/refs/heads/main/security/littlefish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Financial Services
- Merchant Services
- Payments
- Fintech
- Commerce
- Enterprise Platform
---
