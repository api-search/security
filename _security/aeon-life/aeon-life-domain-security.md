---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aeonlife.com.cn
  spf: true
hosts:
- cert_expires: Jan 31 08:39:58 2027 GMT
  host: www.aeonlife.com.cn
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aeon Life Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aeon Life, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aeon Life
provider_slug: aeon-life
slug: aeon-life-domain-security
source_filename: aeon-life-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aeonlife.com.cn\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 31 08:39:58 2027 GMT\n  hsts: null\ndomains:\n- domain: aeonlife.com.cn\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aeon-life/refs/heads/main/security/aeon-life-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Insurance
- Life Insurance
- Health Insurance
- Financial Services
- China
- Consumer
---
