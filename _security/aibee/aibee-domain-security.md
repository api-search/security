---
description: ''
domains:
- caa:
  - aibee.cn.a.bdydns.com.
  - opencdn.jomodns.com.
  dmarc: false
  dnssec: true
  domain: aibee.cn
  spf: false
hosts:
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: www.aibee.cn
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: map.aibee.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Mar  7 23:59:59 2027 GMT
  host: deploy.aibee.cn
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aibee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aibee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Aibee
provider_slug: aibee
slug: aibee-domain-security
source_filename: aibee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aibee.cn\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n- host: map.aibee.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\n- host: deploy.aibee.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aibee.cn\n  dnssec: true\n  caa:\n  - aibee.cn.a.bdydns.com.\n  - opencdn.jomodns.com.\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aibee/refs/heads/main/security/aibee-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Artificial Intelligence
- Computer-Vision
- Indoor Mapping
- Indoor Navigation
- Augmented Reality
- Retail Technology
- Commercial Real Estate
- Smart Parking
- Location Services
- SDK
- China
---
