---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cratejoy.com
  spf: true
hosts:
- cert_expires: Sep 14 13:53:33 2026 GMT
  host: www.cratejoy.com
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cratejoy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cratejoy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cratejoy
provider_slug: cratejoy
slug: cratejoy-domain-security
source_filename: cratejoy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cratejoy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:53:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: cratejoy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cratejoy/refs/heads/main/security/cratejoy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Ecommerce
- Subscriptions
- Subscription Boxes
- Marketplace
- Payments
- Orders
- Webhooks
- REST
---
