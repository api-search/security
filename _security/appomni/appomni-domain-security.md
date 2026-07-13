---
api_specs:
- filename: appomni-openapi.yaml
  format: yaml
  label: AppOmni API
  slug: appomni-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/openapi/appomni-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: appomni.com
  spf: true
hosts:
- cert_expires: Sep 13 22:28:55 2026 GMT
  host: www.appomni.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 03:19:51 2026 GMT
  host: api.appomni.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Appomni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AppOmni, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AppOmni
provider_slug: appomni
slug: appomni-domain-security
source_filename: appomni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.appomni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 22:28:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: api.appomni.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 03:19:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: appomni.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appomni/refs/heads/main/security/appomni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- SaaS Security
- Compliance
- Threat Detection
- CASB
- Zero Trust
---
