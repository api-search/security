---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: woowahan.com
  spf: true
hosts:
- cert_expires: Dec  1 23:59:59 2026 GMT
  host: woowahan.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Woowa Brothers Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Woowa Brothers, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Woowa Brothers
provider_slug: woowa-brothers
slug: woowa-brothers-domain-security
source_filename: woowa-brothers-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: woowahan.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: woowahan.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woowa-brothers/refs/heads/main/security/woowa-brothers-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Technology
- Food Delivery
- Quick Commerce
- Logistics
- Mobile Apps
- South Korea
- E-Commerce
---
