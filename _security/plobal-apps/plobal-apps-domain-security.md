---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: plobalapps.com
  spf: true
hosts:
- cert_expires: Mar 15 23:59:59 2027 GMT
  host: www.plobalapps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plobal Apps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Plobal Apps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Plobal Apps
provider_slug: plobal-apps
slug: plobal-apps-domain-security
source_filename: plobal-apps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plobalapps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: plobalapps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plobal-apps/refs/heads/main/security/plobal-apps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Cloud
- Mobile
- eCommerce
- Shopify
- Mobile Commerce
- Push Notifications
- App Builder
---
