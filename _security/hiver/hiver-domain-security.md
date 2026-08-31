---
api_specs:
- filename: hiver-conversations-api-openapi.yml
  format: yaml
  label: Hiver Conversations API
  slug: hiver-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiver/refs/heads/main/openapi/hiver-conversations-api-openapi.yml
- filename: hiver-inbox-api-openapi.yml
  format: yaml
  label: Hiver Inbox API
  slug: hiver-inbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hiver/refs/heads/main/openapi/hiver-inbox-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hiverhq.com
  spf: true
hosts:
- cert_expires: Sep 25 21:58:47 2026 GMT
  host: hiverhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 17:38:44 2026 GMT
  host: developer.hiverhq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  3 23:59:59 2026 GMT
  host: api2.hiverhq.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hiver Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hiver, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hiver
provider_slug: hiver
slug: hiver-domain-security
source_filename: hiver-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hiverhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 21:58:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.hiverhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 17:38:44 2026 GMT\n  hsts: null\n- host: api2.hiverhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hiverhq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hiver/refs/heads/main/security/hiver-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Service
- Help Desk
- Shared Inbox
- Email
- Ticketing
- Customer-Support
- Collaboration
- Gmail
- Google Workspace
- Omnichannel
- Live Chat
- Software-as-a-Service
- Artificial Intelligence
---
