---
api_specs:
- filename: devportal-factiva-products
  format: yaml
  label: Dow Jones Developer Platform
  slug: dow-jones-developer-platform
  spec_type: Postman
  url: https://www.postman.com/dj-cse/workspace/devportal-factiva-products
- filename: dow-jones-developer-platform-newswires-real-time-api-openapi.yml
  format: yaml
  label: Dow Jones Newswires Real-Time API
  slug: newswires-real-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-newswires-real-time-api-openapi.yml
- filename: dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
  format: yaml
  label: Dow Jones Newswires Top Stories API
  slug: newswires-top-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-newswires-top-stories-api-openapi.yml
- filename: dow-jones-developer-platform-calendar-live-api-openapi.yml
  format: yaml
  label: Dow Jones Calendar Live API
  slug: calendar-live-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-calendar-live-api-openapi.yml
- filename: dow-jones-developer-platform-factiva-content-api-openapi.yml
  format: yaml
  label: Factiva Content API
  slug: factiva-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-factiva-content-api-openapi.yml
- filename: dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
  format: yaml
  label: Factiva Newsletters API
  slug: factiva-newsletters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-factiva-newsletters-api-openapi.yml
- filename: dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
  format: yaml
  label: Dow Jones RiskCenter Third Party Platform API
  slug: riskcenter-third-party-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/openapi/dow-jones-developer-platform-riskcenter-third-party-api-0-2-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dowjones.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: www.dowjones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: developer.dowjones.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: api.dowjones.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Dow Jones Developer Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dow Jones Developer Platform, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Dow Jones Developer Platform
provider_slug: dow-jones-developer-platform
slug: dow-jones-developer-platform-domain-security
source_filename: dow-jones-developer-platform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dowjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: developer.dowjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: false\n- host: api.dowjones.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: dowjones.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dow-jones-developer-platform/refs/heads/main/security/dow-jones-developer-platform-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Data
- Compliance
- Financial
- Market Data
- News
- Risk and Compliance
- Screening
- Sanctions
---
