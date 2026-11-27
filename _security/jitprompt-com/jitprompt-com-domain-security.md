---
api_specs:
- filename: jitprompt-com-account-api-openapi.yml
  format: yaml
  label: jitprompt Account API
  slug: jitprompt-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-account-api-openapi.yml
- filename: jitprompt-com-documents-api-openapi.yml
  format: yaml
  label: jitprompt Documents API
  slug: jitprompt-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-documents-api-openapi.yml
- filename: jitprompt-com-pinned-documents-api-openapi.yml
  format: yaml
  label: jitprompt Pinned documents API
  slug: jitprompt-com-pinned-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-pinned-documents-api-openapi.yml
- filename: jitprompt-com-versions-api-openapi.yml
  format: yaml
  label: jitprompt Versions API
  slug: jitprompt-com-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-versions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: jitprompt.com
  spf: true
hosts:
- cert_expires: Apr 25 23:59:59 2027 GMT
  host: jitprompt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: jitprompt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for jitprompt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: jitprompt
provider_slug: jitprompt-com
slug: jitprompt-com-domain-security
source_filename: jitprompt-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jitprompt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: jitprompt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/jitprompt-com/security/jitprompt-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
---
