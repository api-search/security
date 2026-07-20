---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opencommercegroup.com
  spf: false
hosts:
- cert_expires: Sep 23 17:54:13 2026 GMT
  host: opencommercegroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Beeketing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beeketing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Beeketing
provider_slug: beeketing
slug: beeketing-domain-security
source_filename: beeketing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opencommercegroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 17:54:13 2026 GMT\n  hsts: false\ndomains:\n- domain: opencommercegroup.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beeketing/refs/heads/main/security/beeketing-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-commerce
- Cross-border Commerce
- Marketing
- Shopify Apps
- REST API
- OAuth
- Webhooks
- Themes
- Payments
---
