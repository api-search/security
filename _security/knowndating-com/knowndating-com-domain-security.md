---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: knowndating.com
  spf: true
hosts:
- cert_expires: Feb 12 23:07:35 2027 GMT
  host: www.knowndating.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Knowndating Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Known, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Known
provider_slug: knowndating-com
slug: knowndating-com-domain-security
source_filename: knowndating-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.knowndating.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 23:07:35 2027 GMT\n  hsts: null\ndomains:\n- domain: knowndating.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/knowndating-com/security/knowndating-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
