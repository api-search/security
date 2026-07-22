---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: stacksocial.com
  spf: true
hosts:
- cert_expires: Sep 29 20:46:49 2026 GMT
  host: stacksocial.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stacksocial Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for StackSocial, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: StackSocial
provider_slug: stacksocial
slug: stacksocial-domain-security
source_filename: stacksocial-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stacksocial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 20:46:49 2026 GMT\n  hsts: null\ndomains:\n- domain: stacksocial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stacksocial/refs/heads/main/security/stacksocial-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Marketplace
- Deals
- Digital Goods
- Retail
---
