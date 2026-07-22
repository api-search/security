---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: bsc1.cn
  spf: false
hosts:
- cert_expires: Jan 11 23:59:59 2027 GMT
  host: www.bsc1.cn
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Chinabsc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Beijing Lanweitong Technology (蓝卫通 / BSC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Beijing Lanweitong Technology (蓝卫通 / BSC)
provider_slug: chinabsc
slug: chinabsc-domain-security
source_filename: chinabsc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bsc1.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: bsc1.cn\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chinabsc/refs/heads/main/security/chinabsc-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Health Care
- Telemedicine
- Remote Consultation
- Medical Imaging
- DICOM
- Hospitals
- China
---
