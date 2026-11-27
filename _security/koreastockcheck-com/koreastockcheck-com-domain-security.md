---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: koreastockcheck.com
  spf: true
hosts:
- cert_expires: Jan 14 17:27:36 2027 GMT
  host: koreastockcheck.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: KoreaStockCheck Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KoreaStockCheck, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: KoreaStockCheck
provider_slug: koreastockcheck-com
slug: koreastockcheck-com-domain-security
source_filename: koreastockcheck-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: koreastockcheck.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 14 17:27:36 2027 GMT\n  hsts: false\ndomains:\n- domain: koreastockcheck.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/koreastockcheck-com/security/koreastockcheck-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- filing research
- Korean disclosures
- Dart
- KRX
---
