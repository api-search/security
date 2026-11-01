---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bigmodel.cn
  spf: true
hosts:
- cert_expires: Nov 20 23:59:59 2026 GMT
  host: bigmodel.cn
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigmodel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zhipu AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Zhipu AI
provider_slug: bigmodel
slug: bigmodel-domain-security
source_filename: bigmodel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigmodel.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bigmodel.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bigmodel/security/bigmodel-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
---
