---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: liepin.com
  spf: true
hosts:
- cert_expires: Apr 16 05:43:20 2027 GMT
  host: liepin.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 猎聘 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 猎聘, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: 猎聘
provider_slug: liepin-com
slug: liepin-com-domain-security
source_filename: liepin-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: liepin.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 16 05:43:20 2027 GMT\n  hsts: false\ndomains:\n- domain: liepin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/liepin-com/security/liepin-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
