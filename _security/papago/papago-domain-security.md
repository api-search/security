---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Papago NMT Translation API
  slug: papago-nmt-translation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/papago/refs/heads/main/openapi/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ncloud.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: ncloud-docs.com
  spf: false
hosts:
- cert_expires: Feb 23 23:59:59 2027 GMT
  host: www.ncloud.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 06:52:21 2026 GMT
  host: api.ncloud-docs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: papago.apigw.ntruss.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Papago Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Papago, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Papago
provider_slug: papago
slug: papago-domain-security
source_filename: papago-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 23 23:59:59 2027 GMT\n  hsts: null\n- host: api.ncloud-docs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 06:52:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: papago.apigw.ntruss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ncloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: ncloud-docs.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/papago/refs/heads/main/security/papago-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Translation
- Natural Language Processing
- Machine Translation
- Neural Machine Translation
- Korean
- Asian Languages
- Localization
- Language Detection
---
