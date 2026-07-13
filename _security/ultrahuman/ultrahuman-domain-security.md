---
api_specs:
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman Metrics API
  slug: ultrahuman-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman CGM (Glucose) API
  slug: ultrahuman-cgm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman User Info API
  slug: ultrahuman-user-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
- filename: ultrahuman-openapi.yml
  format: yaml
  label: Ultrahuman OAuth 2.0 API
  slug: ultrahuman-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/openapi/ultrahuman-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "certainly.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ultrahuman.com
  spf: true
hosts:
- cert_expires: Sep 30 05:14:46 2026 GMT
  host: www.ultrahuman.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: vision.ultrahuman.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep  3 07:14:12 2026 GMT
  host: partner.ultrahuman.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ultrahuman Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ultrahuman, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ultrahuman
provider_slug: ultrahuman
slug: ultrahuman-domain-security
source_filename: ultrahuman-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ultrahuman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:14:46 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: vision.ultrahuman.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: false\n- host: partner.ultrahuman.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 07:14:12 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: ultrahuman.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"certainly.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ultrahuman/refs/heads/main/security/ultrahuman-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wearables
- Smart Ring
- Health
- Metabolic Health
- Sleep
- HRV
- Recovery
- CGM
- Glucose
- Digital Health
---
