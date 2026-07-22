---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: singular.net
  spf: true
hosts:
- cert_expires: Sep 28 14:27:51 2026 GMT
  host: singular.net
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Singular Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Singular, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Singular
provider_slug: singular
slug: singular-domain-security
source_filename: singular-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: singular.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 14:27:51 2026 GMT\n  hsts: false\ndomains:\n- domain: singular.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/singular/refs/heads/main/security/singular-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketing Analytics
- Mobile Attribution
- Attribution
- Marketing
- Advertising
- Analytics
- Mobile Measurement Partner
- SKAdNetwork
- Deep Linking
- Fraud Prevention
- ETL
---
