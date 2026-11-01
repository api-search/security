---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: sparkfun.com
  spf: true
hosts:
- cert_expires: Jan  6 13:33:48 2027 GMT
  host: www.sparkfun.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sparkfun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SparkFun Electronics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SparkFun Electronics
provider_slug: sparkfun
slug: sparkfun-domain-security
source_filename: sparkfun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sparkfun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 13:33:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: sparkfun.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sparkfun/security/sparkfun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Electronics
- Retail
- Maker
- Education
- Community
---
