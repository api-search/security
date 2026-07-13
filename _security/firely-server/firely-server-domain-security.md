---
api_specs:
- filename: simplifier-package-api-openapi.yml
  format: yaml
  label: Simplifier.net FHIR Package API
  slug: simplifier-package-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/firely-server/refs/heads/main/openapi/simplifier-package-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: fire.ly
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: simplifier.net
  spf: true
hosts:
- cert_expires: Sep  1 23:14:06 2026 GMT
  host: fire.ly
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 01:52:57 2026 GMT
  host: docs.fire.ly
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: packages.simplifier.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Firely Server Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Firely, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Firely
provider_slug: firely-server
slug: firely-server-domain-security
source_filename: firely-server-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fire.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 23:14:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.fire.ly\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 01:52:57 2026 GMT\n  hsts: false\n- host: packages.simplifier.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fire.ly\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: simplifier.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/firely-server/refs/heads/main/security/firely-server-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- FHIR
- HL7
- Healthcare
- Health IT
- Interoperability
- Clinical Data
- FHIR Server
- Vonk
- Simplifier
- Forge
- Terminology
- SMART on FHIR
- Bulk Data
- CDS Hooks
- Implementation Guides
- .NET SDK
- CQL
- Profile Registry
---
