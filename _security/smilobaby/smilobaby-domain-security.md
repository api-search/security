---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: smilobaby.com
  spf: true
hosts:
- cert_expires: Aug 31 09:44:28 2026 GMT
  host: smilobaby.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smilobaby Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smilobaby, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Smilobaby
provider_slug: smilobaby
slug: smilobaby-domain-security
source_filename: smilobaby-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: smilobaby.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:44:28 2026 GMT\n  hsts: false\ndomains:\n- domain: smilobaby.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smilobaby/refs/heads/main/security/smilobaby-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Baby Products
- Consumer
- E-Commerce
- Retail
- Parenting
- Direct-to-Consumer
---
