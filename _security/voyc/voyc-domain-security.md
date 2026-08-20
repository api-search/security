---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: voyc.ai
  spf: true
hosts:
- cert_expires: Nov  7 08:08:20 2026 GMT
  host: voyc.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 25 23:59:59 2026 GMT
  host: help.voyc.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: api.app.voyc.ai
  hsts: true
  hsts_header: max-age=60; includeSubDomains; preload
  hsts_max_age: 60
  hsts_note: 'Corrected by hand after the script recorded null: HEAD https://api.app.voyc.ai/ and GET https://api.app.voyc.ai/v3/organisation/ both return the header. max-age=60 is far below the 31536000 the HSTS preload list requires, so the preload directive is not effective and the protection window is one minute.'
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Voyc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Voyc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Voyc
provider_slug: voyc
slug: voyc-domain-security
source_filename: voyc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: voyc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 08:08:20 2026 GMT\n  hsts: false\n- host: help.voyc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 23:59:59 2026 GMT\n  hsts: false\n- host: api.app.voyc.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 60\n  hsts_header: 'max-age=60; includeSubDomains; preload'\n  hsts_note: >-\n    Corrected by hand after the script recorded null: HEAD https://api.app.voyc.ai/\n    and GET https://api.app.voyc.ai/v3/organisation/ both return the header. max-age=60\n    is far below the 31536000 the HSTS preload list requires, so the preload directive\n    is not effective and the protection window is one minute.\ndomains:\n- domain: voyc.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/voyc/refs/heads/main/security/voyc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Conversation Intelligence
- Compliance
- Call Monitoring
- Speech Analytics
- Contact Centers
- Financial-Services
- Artificial Intelligence
---
