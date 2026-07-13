---
api_specs:
- filename: openapi-directory
  format: yaml
  label: Aserto Authorizer API
  slug: aserto-authorizer-api
  spec_type: OpenAPI
  url: https://github.com/aserto-dev/openapi-directory
- filename: openapi-directory
  format: yaml
  label: Aserto Directory API
  slug: aserto-directory-api
  spec_type: OpenAPI
  url: https://github.com/aserto-dev/openapi-directory
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aserto.com
  spf: true
hosts:
- cert_expires: Oct  2 05:53:41 2026 GMT
  host: www.aserto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 18:53:51 2026 GMT
  host: docs.aserto.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: authorizer.prod.aserto.com
  https: false
kind: domain-security
layout: security
method: probed
name: Aserto Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aserto, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Aserto
provider_slug: aserto
slug: aserto-domain-security
source_filename: aserto-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aserto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 05:53:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.aserto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 18:53:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: authorizer.prod.aserto.com\n  https: false\ndomains:\n- domain: aserto.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/security/aserto-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Authorization
- Fine-Grained Access Control
- RBAC
- ABAC
- ReBAC
- Policy
- Open Policy Agent
- OPA
- Cloud-Native
- Security
---
