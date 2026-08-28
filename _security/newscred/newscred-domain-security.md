---
api_specs:
- filename: newscred-cmp-open-api-openapi.json
  format: json
  label: Optimizely CMP Open API v3
  slug: optimizely-cmp-open-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-cmp-open-api-openapi.json
- filename: newscred-welcome-open-api-openapi.yml
  format: yaml
  label: Welcome Open API v3 (legacy)
  slug: welcome-open-api-v3-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/openapi/newscred-welcome-open-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optimizely.com
  spf: true
hosts:
- cert_expires: Nov 21 14:03:17 2026 GMT
  host: www.optimizely.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:32:33 2026 GMT
  host: docs.developers.optimizely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: api.cmp.optimizely.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Newscred Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Newscred, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Newscred
provider_slug: newscred
slug: newscred-domain-security
source_filename: newscred-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optimizely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 14:03:17 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.developers.optimizely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cmp.optimizely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: optimizely.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newscred/refs/heads/main/security/newscred-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Content Marketing
- Content Management
- Digital Asset Management
- Marketing
- Marketing Resource Management
- Workflow
- Publishing
- Webhooks
- Acquired
---
