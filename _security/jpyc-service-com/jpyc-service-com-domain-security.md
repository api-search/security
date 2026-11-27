---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jpyc-service.com
  spf: true
hosts:
- cert_expires: Dec 20 07:37:24 2026 GMT
  host: jpyc-service.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: JPYC株式会社 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for JPYC株式会社, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: JPYC株式会社
provider_slug: jpyc-service-com
slug: jpyc-service-com-domain-security
source_filename: jpyc-service-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jpyc-service.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 07:37:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: jpyc-service.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jpyc-service-com/security/jpyc-service-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- ECプラットフォーム
---
