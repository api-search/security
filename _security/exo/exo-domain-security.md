---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: exo.inc
  spf: true
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: exoworks.inc
  spf: false
hosts:
- cert_expires: Sep 25 20:46:56 2026 GMT
  host: www.exo.inc
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:43:17 2026 GMT
  host: support.exo.inc
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 259200
  https: true
  note: Zendesk-hosted help center
  tls_version: TLSv1.3
- cert_expires: Oct  2 22:48:32 2026 GMT
  host: store.exo.inc
  hsts: true
  hsts_max_age: 7889238
  https: true
  note: Shopify-hosted store
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: cloud.exoworks.inc
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: true
  https: true
  note: Exo Works web application (single-page app shell)
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: api.prod.exoworks.inc
  hsts: null
  https: true
  note: Exo Works production API host (AWS API Gateway behind CloudFront). Anonymous GET / returns HTTP 403 {"message":"Forbidden"} with x-amzn-errortype ForbiddenException. Private product backend - no public documentation, no public specification.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Exo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Exo, probed live across 5 host(s) and 2 registrable domain(s). 5 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Exo
provider_slug: exo
slug: exo-domain-security
source_filename: exo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml hosts + observed Exo product hosts\nhosts:\n- host: www.exo.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:46:56 2026 GMT\n  hsts: null\n- host: support.exo.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:43:17 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n  hsts_include_subdomains: true\n  note: Zendesk-hosted help center\n- host: store.exo.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 22:48:32 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\n  note: Shopify-hosted store\n- host: cloud.exoworks.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  note: Exo Works web application (single-page app shell)\n- host: api.prod.exoworks.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16\
  \ 23:59:59 2026 GMT\n  hsts: null\n  note: 'Exo Works production API host (AWS API Gateway behind CloudFront). Anonymous\n    GET / returns HTTP 403 {\"message\":\"Forbidden\"} with x-amzn-errortype ForbiddenException.\n    Private product backend - no public documentation, no public specification.'\ndomains:\n- domain: exo.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: exoworks.inc\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exo/refs/heads/main/security/exo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Medical Imaging
- Ultrasound
- Point of Care
- Artificial Intelligence
- Medical Devices
- DICOM
- HL7
---
