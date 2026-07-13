---
api_specs:
- filename: api
  format: yaml
  label: Oso Cloud Authorization API
  slug: oso-cloud-authorization-api
  spec_type: OpenAPI
  url: https://www.osohq.com/docs/reference/api
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: osohq.com
  spf: true
hosts:
- cert_expires: Aug 10 10:46:38 2026 GMT
  host: www.osohq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 26 23:59:59 2026 GMT
  host: api.osohq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Oso Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Oso Cloud, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Oso Cloud
provider_slug: oso
slug: oso-domain-security
source_filename: oso-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.osohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 10:46:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.osohq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: osohq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oso/refs/heads/main/security/oso-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authorization
- Access Control
- RBAC
- ReBAC
- ABAC
- Permissions
- Policy
- Security
- Identity
---
