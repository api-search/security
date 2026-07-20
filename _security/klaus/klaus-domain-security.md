---
api_specs:
- filename: klaus-public-export-api-openapi-original.json
  format: json
  label: Klaus Public Export API
  slug: public-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaus/refs/heads/main/openapi/klaus-public-export-api-openapi-original.json
- filename: klaus-public-import-api-openapi-original.json
  format: json
  label: Klaus Public Import API
  slug: public-import-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaus/refs/heads/main/openapi/klaus-public-import-api-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: klausapp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zendesk.com
  spf: true
hosts:
- cert_expires: Sep 14 12:21:03 2026 GMT
  host: www.klausapp.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 06:00:46 2026 GMT
  host: pub.klausapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 14:46:45 2026 GMT
  host: yoursubdomain.zendesk.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klaus Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klaus, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Klaus
provider_slug: klaus
slug: klaus-domain-security
source_filename: klaus-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klausapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 12:21:03 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: pub.klausapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 06:00:46 2026 GMT\n  hsts: false\n- host: yoursubdomain.zendesk.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 14:46:45 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: klausapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: zendesk.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaus/refs/heads/main/security/klaus-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Quality Assurance
- Customer Support
- Customer Experience
- Conversation Analytics
- Contact Center
- Coaching
- Artificial Intelligence
- SaaS
---
