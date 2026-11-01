---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: baihe.com
  spf: true
hosts:
- cert_expires: Dec 27 03:06:26 2026 GMT
  host: i.baihe.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Baihe Holding Corporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Baihe Holding Corporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Baihe Holding Corporation
provider_slug: baihe-holding-corporation
slug: baihe-holding-corporation-domain-security
source_filename: baihe-holding-corporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: i.baihe.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 03:06:26 2026 GMT\n  hsts: false\ndomains:\n- domain: baihe.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/baihe-holding-corporation/security/baihe-holding-corporation-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
