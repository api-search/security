---
api_specs:
- filename: searchstax-provisioning-openapi.yml
  format: yaml
  label: SearchStax Provisioning API
  slug: searchstax-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-provisioning-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: searchstax.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: www.searchstax.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: app.searchstax.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- host: search.searchstax.com
  https: false
kind: domain-security
layout: security
method: probed
name: Searchstax Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SearchStax, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SearchStax
provider_slug: searchstax
slug: searchstax-domain-security
source_filename: searchstax-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.searchstax.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\n- host: app.searchstax.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: null\n- host: search.searchstax.com\n  https: false\ndomains:\n- domain: searchstax.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/security/searchstax-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Search
- Solr
- Managed Search
- Search Infrastructure
- Full-Text Search
- Site Search
---
