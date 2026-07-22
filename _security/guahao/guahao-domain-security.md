---
description: ''
domains:
- caa:
  - idc-xy230ba230-bgp.wedoctort.com.
  dmarc: false
  dnssec: true
  domain: guahao.com
  spf: true
hosts:
- cert_expires: Dec 17 23:59:59 2026 GMT
  host: guahao.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Guahao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for guahao, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: guahao
provider_slug: guahao
slug: guahao-domain-security
source_filename: guahao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: guahao.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 17 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: guahao.com\n  dnssec: true\n  caa:\n  - idc-xy230ba230-bgp.wedoctort.com.\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guahao/refs/heads/main/security/guahao-domain-security.yml
summary_line: TLSv1.2 · DNSSEC
tags:
- Company
- Healthcare
- Digital Health
- Telemedicine
- Appointment Booking
- China
- Internet Hospital
---
