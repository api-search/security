---
api_specs:
- filename: fossil-scm-home-api-openapi.yml
  format: yaml
  label: Fossil SCM Home API
  slug: fossil-scm-home-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossil-scm/refs/heads/main/openapi/fossil-scm-home-api-openapi.yml
- filename: fossil-scm-json-api-openapi.yml
  format: yaml
  label: Fossil SCM JSON API
  slug: fossil-scm-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossil-scm/refs/heads/main/openapi/fossil-scm-json-api-openapi.yml
- filename: fossil-scm-wikis-api-openapi.yml
  format: yaml
  label: Fossil SCM Wikis API
  slug: fossil-scm-wikis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fossil-scm/refs/heads/main/openapi/fossil-scm-wikis-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fossil-scm.org
  spf: true
hosts:
- cert_expires: Oct 30 01:03:34 2026 GMT
  host: fossil-scm.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fossil Scm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fossil SCM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Fossil SCM
provider_slug: fossil-scm
slug: fossil-scm-domain-security
source_filename: fossil-scm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fossil-scm.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 01:03:34 2026 GMT\n  hsts: false\ndomains:\n- domain: fossil-scm.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fossil-scm/refs/heads/main/security/fossil-scm-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Version Control
- Open Source
- SCM
- Distributed
- Configuration Management
---
