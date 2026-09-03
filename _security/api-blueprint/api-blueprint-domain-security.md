---
api_specs:
- filename: api-blueprint-parsing-service-openapi.yml
  format: yaml
  label: API Blueprint API
  slug: api-blueprint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/api-blueprint/refs/heads/main/openapi/api-blueprint-parsing-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apiblueprint.org
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiary.io
  spf: true
hosts:
- cert_expires: Nov 25 15:56:18 2026 GMT
  host: apiblueprint.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  6 23:59:59 2027 GMT
  host: apiblueprintapi.docs.apiary.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: api.apiblueprint.org
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Api Blueprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for API Blueprint, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: API Blueprint
provider_slug: api-blueprint
slug: api-blueprint-domain-security
source_filename: api-blueprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiblueprint.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 25 15:56:18 2026 GMT\n  hsts: false\n- host: apiblueprintapi.docs.apiary.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  6 23:59:59 2027 GMT\n  hsts: false\n- host: api.apiblueprint.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: apiblueprint.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: apiary.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-blueprint/refs/heads/main/security/api-blueprint-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- API Design
- Specification Language
- Markdown
- Documentation
- API Description Language
- Parsing
- Open Source
- Developer Tools
---
