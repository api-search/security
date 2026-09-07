---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: activon-global.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: activon.kr
  spf: true
hosts:
- cert_expires: Nov 28 17:50:21 2026 GMT
  host: www.activon-global.com
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.activon.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Activeon8016 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACTIVON Co., Ltd., probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ACTIVON Co., Ltd.
provider_slug: activeon8016
slug: activeon8016-domain-security
source_filename: activeon8016-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.activon-global.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 17:50:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\n- host: www.activon.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: activon-global.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: activon.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activeon8016/refs/heads/main/security/activeon8016-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cosmetics
- Chemicals
- Ingredients
- Materials
- Manufacturing
- Biotechnology
- Micro-Encapsulation
- Pigments
- South Korea
---
