---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: datablau.cn
  spf: false
hosts:
- cert_expires: Nov  4 15:59:59 2026 GMT
  host: datablau.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Datablau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Datablau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Datablau
provider_slug: datablau
slug: datablau-domain-security
source_filename: datablau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: datablau.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov  4 15:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: datablau.cn\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/datablau/security/datablau-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
---
