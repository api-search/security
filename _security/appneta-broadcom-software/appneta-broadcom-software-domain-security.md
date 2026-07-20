---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appneta.com
  spf: true
hosts:
- cert_expires: Mar 20 23:59:59 2027 GMT
  host: www.appneta.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Appneta Broadcom Software Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppNeta (Broadcom Software), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppNeta (Broadcom Software)
provider_slug: appneta-broadcom-software
slug: appneta-broadcom-software-domain-security
source_filename: appneta-broadcom-software-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appneta.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appneta.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appneta-broadcom-software/refs/heads/main/security/appneta-broadcom-software-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Network Monitoring
- Network Performance
- Observability
- Application Performance
- Digital Experience Monitoring
- Synthetic Monitoring
- IT Operations
- Broadcom
- Ai Infrastructure
---
