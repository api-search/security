---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kitbench.net
  spf: true
hosts:
- cert_expires: Dec 31 06:51:36 2026 GMT
  host: kitbench.net
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: 合同会社AI Content Hub Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 合同会社AI Content Hub, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 合同会社AI Content Hub
provider_slug: kitbench-net
slug: kitbench-net-domain-security
source_filename: kitbench-net-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kitbench.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 06:51:36 2026 GMT\n  hsts: false\ndomains:\n- domain: kitbench.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kitbench-net/security/kitbench-net-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
