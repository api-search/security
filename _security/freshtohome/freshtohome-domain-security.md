---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: freshtohome.com
  spf: true
hosts:
- cert_expires: Sep 26 22:38:20 2026 GMT
  host: www.freshtohome.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freshtohome Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FreshToHome, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FreshToHome
provider_slug: freshtohome
slug: freshtohome-domain-security
source_filename: freshtohome-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freshtohome.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 22:38:20 2026 GMT\n  hsts: false\ndomains:\n- domain: freshtohome.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freshtohome/refs/heads/main/security/freshtohome-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- E-Commerce
- Food and Beverage
- Grocery
- Retail
- Direct to Consumer
- Supply Chain
- Delivery
- India
- United Arab Emirates
---
