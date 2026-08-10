---
api_specs:
- filename: disqo-audience-api-postman.json
  format: json
  label: DISQO Audience Projects API
  slug: disqo-audience-projects-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/disqo/refs/heads/main/postman/disqo-audience-api-postman.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: disqo.com
  spf: true
hosts:
- cert_expires: Oct  8 14:49:23 2026 GMT
  host: www.disqo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 14:49:23 2026 GMT
  host: developer.disqo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 14:49:23 2026 GMT
  host: projects-api.audience.disqo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Disqo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DISQO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DISQO
provider_slug: disqo
slug: disqo-domain-security
source_filename: disqo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.disqo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:49:23 2026 GMT\n  hsts: null\n- host: developer.disqo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:49:23 2026 GMT\n  hsts: null\n- host: projects-api.audience.disqo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 14:49:23 2026 GMT\n  hsts: null\ndomains:\n- domain: disqo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/disqo/refs/heads/main/security/disqo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Audience
- Market Research
- Surveys
- Consumer Insights
- Advertising Measurement
- Panel
- Brand Lift
- Data
- Analytics
---
