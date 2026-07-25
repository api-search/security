---
api_specs:
- filename: internet-engineering-task-force-documents-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Documents API
  slug: internet-engineering-task-force-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-documents-api-openapi.yml
- filename: internet-engineering-task-force-framework-api-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Framework API API
  slug: internet-engineering-task-force-framework-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-framework-api-api-openapi.yml
- filename: internet-engineering-task-force-identity-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Identity API
  slug: internet-engineering-task-force-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-identity-api-openapi.yml
- filename: internet-engineering-task-force-iesg-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force IESG API
  slug: internet-engineering-task-force-iesg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-iesg-api-openapi.yml
- filename: internet-engineering-task-force-meetings-api-openapi.yml
  format: yaml
  label: Internet Engineering Task Force Meetings API
  slug: internet-engineering-task-force-meetings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/openapi/internet-engineering-task-force-meetings-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: ietf.org
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rfc-editor.org
  spf: true
hosts:
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: www.ietf.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:01:07 2026 GMT
  host: datatracker.ietf.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 05:02:36 2026 GMT
  host: www.rfc-editor.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Internet Engineering Task Force Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Internet Engineering Task Force, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Internet Engineering Task Force
provider_slug: internet-engineering-task-force
slug: internet-engineering-task-force-domain-security
source_filename: internet-engineering-task-force-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: false\n- host: datatracker.ietf.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:01:07 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\n- host: www.rfc-editor.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 05:02:36 2026 GMT\n  hsts: false\ndomains:\n- domain: ietf.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rfc-editor.org\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/internet-engineering-task-force/refs/heads/main/security/internet-engineering-task-force-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Internet
- Protocols
- RFC
- Standards
- Working Groups
---
