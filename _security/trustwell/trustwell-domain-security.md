---
api_specs:
- filename: trustwell-foodlogiq-openapi.yml
  format: yaml
  label: Trustwell FoodLogiQ API
  slug: trustwell-foodlogiq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trustwell/refs/heads/main/openapi/trustwell-foodlogiq-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: trustwell.com
  spf: true
hosts:
- cert_expires: Sep 25 08:39:56 2026 GMT
  host: www.trustwell.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: docs.trustwell.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 11 16:11:50 2026 GMT
  host: api.trustwell.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Trustwell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trustwell, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Trustwell
provider_slug: trustwell
slug: trustwell-domain-security
source_filename: trustwell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.trustwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:39:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.trustwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: false\n- host: api.trustwell.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 11 16:11:50 2026 GMT\n  hsts: null\ndomains:\n- domain: trustwell.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trustwell/refs/heads/main/security/trustwell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Food Industry
- Food Safety
- Nutrition
- Supply Chain
- Food Labeling
- Traceability
- Compliance
- Food Technology
---
