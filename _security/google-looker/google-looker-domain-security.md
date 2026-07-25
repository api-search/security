---
api_specs:
- filename: google-looker-authentication-api-openapi.yml
  format: yaml
  label: Google Looker Authentication API
  slug: google-looker-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker/refs/heads/main/openapi/google-looker-authentication-api-openapi.yml
- filename: google-looker-looks-api-openapi.yml
  format: yaml
  label: Google Looker Looks API
  slug: google-looker-looks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker/refs/heads/main/openapi/google-looker-looks-api-openapi.yml
- filename: google-looker-users-api-openapi.yml
  format: yaml
  label: Google Looker Users API
  slug: google-looker-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-looker/refs/heads/main/openapi/google-looker-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: looker.com
  spf: true
hosts:
- cert_expires: Sep 14 08:35:22 2026 GMT
  host: cloud.google.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: your-instance.cloud.looker.com
  https: false
- cert_expires: Sep 14 08:37:17 2026 GMT
  host: looker.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Google Looker Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Looker, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Looker
provider_slug: google-looker
slug: google-looker-domain-security
source_filename: google-looker-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloud.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:35:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: your-instance.cloud.looker.com\n  https: false\n- host: looker.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 08:37:17 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: looker.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-looker/refs/heads/main/security/google-looker-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags: []
---
