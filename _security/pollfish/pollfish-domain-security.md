---
api_specs:
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Apps API
  slug: pollfish-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Performance API
  slug: pollfish-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Revenue API
  slug: pollfish-revenue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Respondent Demographics API
  slug: pollfish-respondent-demographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish User Logs API
  slug: pollfish-user-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Survey Distribution and Offerwall API
  slug: pollfish-survey-distribution-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
- filename: pollfish-openapi.yml
  format: yaml
  label: Pollfish Server-to-Server Callbacks
  slug: pollfish-s2s-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/openapi/pollfish-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pollfish.com
  spf: true
hosts:
- cert_expires: Feb  8 09:35:19 2027 GMT
  host: www.pollfish.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  8 09:35:19 2027 GMT
  host: wss.pollfish.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Pollfish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Pollfish, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Pollfish
provider_slug: pollfish
slug: pollfish-domain-security
source_filename: pollfish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.pollfish.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 09:35:19 2027 GMT\n  hsts: false\n- host: wss.pollfish.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  8 09:35:19 2027 GMT\n  hsts: false\ndomains:\n- domain: pollfish.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pollfish/refs/heads/main/security/pollfish-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Surveys
- Market Research
- Mobile
- Monetization
- Offerwall
- Rewarded Ads
- Prodege
---
