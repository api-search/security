---
api_specs:
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Stats API
  slug: simpleanalytics-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Export API
  slug: simpleanalytics-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Events API
  slug: simpleanalytics-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
- filename: simpleanalytics-openapi.yml
  format: yaml
  label: Simple Analytics Websites API
  slug: simpleanalytics-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/openapi/simpleanalytics-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: simpleanalytics.com
  spf: true
hosts:
- cert_expires: Aug 21 21:48:51 2026 GMT
  host: www.simpleanalytics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 22:28:50 2026 GMT
  host: docs.simpleanalytics.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:48:51 2026 GMT
  host: simpleanalytics.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Simpleanalytics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Simple Analytics, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Simple Analytics
provider_slug: simpleanalytics
slug: simpleanalytics-domain-security
source_filename: simpleanalytics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.simpleanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:48:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.simpleanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 22:28:50 2026 GMT\n  hsts: false\n- host: simpleanalytics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 21:48:51 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: simpleanalytics.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simpleanalytics/refs/heads/main/security/simpleanalytics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Analytics
- Web Analytics
- Privacy
- Cookieless
- GDPR
---
