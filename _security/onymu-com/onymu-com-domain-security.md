---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: onymu.com
  spf: true
hosts:
- cert_expires: Jan 25 10:11:27 2027 GMT
  host: onymu.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: onymu-com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for onymu-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: onymu-com
provider_slug: onymu-com
slug: onymu-com-domain-security
source_filename: onymu-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onymu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 10:11:27 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: onymu.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/onymu-com/security/onymu-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
