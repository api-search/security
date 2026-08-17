---
api_specs:
- filename: opal-v2-openapi.yml
  format: yaml
  label: Opal API v2
  slug: opal-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-v2-openapi.yml
- filename: opal-v3-openapi.yml
  format: yaml
  label: Opal API v3
  slug: opal-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-v3-openapi.yml
- filename: opal-asgard-bff-openapi.yml
  format: yaml
  label: Opal Asgard BFF API
  slug: opal-asgard-bff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/openapi/opal-asgard-bff-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: workwithopal.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ouropal.com
  spf: true
hosts:
- cert_expires: Sep 24 10:29:47 2026 GMT
  host: www.workwithopal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: login.ouropal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opal, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Opal
provider_slug: opal
slug: opal-domain-security
source_filename: opal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.workwithopal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 10:29:47 2026 GMT\n  hsts: false\n- host: login.ouropal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: workwithopal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ouropal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opal/refs/heads/main/security/opal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Marketing
- Content Planning
- Marketing Calendar
- Campaign Management
- Collaboration
- SaaS
- Content Marketing
- Editorial Calendar
- Workflow
- Approvals
- Digital Asset Management
- JSON:API
- OAuth 2.0
- OpenAPI
---
