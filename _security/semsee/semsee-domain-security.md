---
api_specs:
- filename: semsee-openapi.yml
  format: yaml
  label: Semsee Submissions API
  slug: semsee-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semsee/refs/heads/main/openapi/semsee-openapi.yml
- filename: semsee-openapi.yml
  format: yaml
  label: Semsee Quotes API
  slug: semsee-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semsee/refs/heads/main/openapi/semsee-openapi.yml
- filename: semsee-openapi.yml
  format: yaml
  label: Semsee Carriers API
  slug: semsee-carriers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semsee/refs/heads/main/openapi/semsee-openapi.yml
- filename: semsee-openapi.yml
  format: yaml
  label: Semsee Webhooks API
  slug: semsee-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/semsee/refs/heads/main/openapi/semsee-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: semsee.com
  spf: true
hosts:
- cert_expires: Feb 14 23:59:59 2027 GMT
  host: www.semsee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 13:43:42 2026 GMT
  host: semsee.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Semsee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Semsee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Semsee
provider_slug: semsee
slug: semsee-domain-security
source_filename: semsee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.semsee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 14 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: semsee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 13:43:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: semsee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/semsee/refs/heads/main/security/semsee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Insurance
- Insurtech
- Commercial Insurance
- Quoting
- Submissions
---
