---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kokkan.co.kr
  spf: true
hosts:
- cert_expires: Feb  7 23:59:59 2027 GMT
  host: kokkan.co.kr
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Kokkanlogis Coltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for KokkanLogis Co.,Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: KokkanLogis Co.,Ltd.
provider_slug: kokkanlogis-coltd
slug: kokkanlogis-coltd-domain-security
source_filename: kokkanlogis-coltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kokkan.co.kr\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  7 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: kokkan.co.kr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kokkanlogis-coltd/refs/heads/main/security/kokkanlogis-coltd-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Logistics
- Self Storage
- Warehousing
- Storage as a Service
- Consumer Services
- Mobile Apps
- South Korea
- Franchise
---
