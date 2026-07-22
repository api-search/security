---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: breadfast.com
  spf: true
hosts:
- cert_expires: Sep 24 17:00:26 2026 GMT
  host: breadfast.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breadfast Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breadfast, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Breadfast
provider_slug: breadfast
slug: breadfast-domain-security
source_filename: breadfast-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breadfast.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:00:26 2026 GMT\n  hsts: false\ndomains:\n- domain: breadfast.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breadfast/refs/heads/main/security/breadfast-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Grocery
- Quick Commerce
- Delivery
- E-Commerce
- Retail
- Fintech
- Egypt
---
