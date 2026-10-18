---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cainiao.com
  spf: true
hosts:
- cert_expires: Jan 11 04:26:26 2027 GMT
  host: www.cainiao.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cainiao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cainiao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cainiao
provider_slug: cainiao
slug: cainiao-domain-security
source_filename: cainiao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cainiao.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 11 04:26:26 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cainiao.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cainiao/refs/heads/main/security/cainiao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Logistics
- E-Commerce
- Supply Chain
- AlibabaGroup
---
