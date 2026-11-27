---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getaroundhongkong.com
  spf: true
hosts:
- cert_expires: Jan  1 15:32:07 2027 GMT
  host: getaroundhongkong.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Get Around Hong Kong Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Get Around Hong Kong, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Get Around Hong Kong
provider_slug: getaroundhongkong-com
slug: getaroundhongkong-com-domain-security
source_filename: getaroundhongkong-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: getaroundhongkong.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 15:32:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: getaroundhongkong.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/getaroundhongkong-com/security/getaroundhongkong-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Transportation
- Transit
- Hong Kong
- Public Transport
- Travel
---
