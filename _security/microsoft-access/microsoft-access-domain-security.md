---
api_specs:
- filename: openapi.json
  format: json
  label: Microsoft Access Database Engine API
  slug: microsoft-access-database-engine-api
  spec_type: OpenAPI
  url: https://example.com/openapi.json
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Access Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Access, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Access
provider_slug: microsoft-access
slug: microsoft-access-domain-security
source_filename: microsoft-access-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-access/refs/heads/main/security/microsoft-access-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Access Database
- Database
- Desktop Database
- Microsoft
- Relational Database
---
