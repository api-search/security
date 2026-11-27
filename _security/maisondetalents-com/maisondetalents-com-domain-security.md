---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maisondetalents.com
  spf: true
hosts:
- cert_expires: Jan 12 09:53:43 2027 GMT
  host: maisondetalents.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 메종 드 탤런트 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 메종 드 탤런트, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 메종 드 탤런트
provider_slug: maisondetalents-com
slug: maisondetalents-com-domain-security
source_filename: maisondetalents-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maisondetalents.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 09:53:43 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: maisondetalents.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/maisondetalents-com/security/maisondetalents-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Recruiting
- Luxury Retail
- South Korea
- JobPlatform
---
