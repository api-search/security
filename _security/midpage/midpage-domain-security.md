---
api_specs:
- filename: midpage-openapi.yml
  format: yaml
  label: Midpage Case Law Search API
  slug: case-law-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-openapi.yml
- filename: midpage-openapi.yml
  format: yaml
  label: Midpage Document Retrieval API
  slug: document-retrieval
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-openapi.yml
- filename: midpage-openapi.yml
  format: yaml
  label: Midpage Citations API
  slug: citations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-openapi.yml
- filename: midpage-openapi.yml
  format: yaml
  label: Midpage Semantic Search API
  slug: semantic-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/openapi/midpage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: midpage.ai
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: apidocumentation.com
  spf: false
hosts:
- cert_expires: Sep  1 01:16:13 2026 GMT
  host: www.midpage.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 17:09:39 2026 GMT
  host: midpage-docs.apidocumentation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:11:26 2026 GMT
  host: app.midpage.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Midpage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Midpage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Midpage
provider_slug: midpage
slug: midpage-domain-security
source_filename: midpage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.midpage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 01:16:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: midpage-docs.apidocumentation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 17:09:39 2026 GMT\n  hsts: false\n- host: app.midpage.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:11:26 2026 GMT\n  hsts: null\ndomains:\n- domain: midpage.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: apidocumentation.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/midpage/refs/heads/main/security/midpage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal
- Case Law
- Legal Research
- Search
- AI
---
