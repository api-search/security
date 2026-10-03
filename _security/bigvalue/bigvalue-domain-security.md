---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bigvalue.ai
  spf: false
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: bigvalue.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bigvalue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bigvalue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Bigvalue
provider_slug: bigvalue
slug: bigvalue-domain-security
source_filename: bigvalue-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bigvalue.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: bigvalue.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bigvalue/refs/heads/main/security/bigvalue-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- PropTech
- Artificial Intelligence
- Real Estate
- Data Analytics
---
