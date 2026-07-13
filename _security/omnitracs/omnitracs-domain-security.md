---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: omnitracs.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: roadnet.com
  spf: true
hosts:
- cert_expires: Aug 14 01:35:36 2026 GMT
  host: www.omnitracs.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: apex-prod-integration.aws.roadnet.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: services.omnitracs.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Omnitracs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Omnitracs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Omnitracs
provider_slug: omnitracs
slug: omnitracs-domain-security
source_filename: omnitracs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.omnitracs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 01:35:36 2026 GMT\n  hsts: false\n- host: apex-prod-integration.aws.roadnet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: null\n- host: services.omnitracs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: omnitracs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: roadnet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnitracs/refs/heads/main/security/omnitracs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fleet Management
- Telematics
- ELD
- Hours of Service
- Transportation
- Routing
- Trucking
- GPS
- Solera
---
