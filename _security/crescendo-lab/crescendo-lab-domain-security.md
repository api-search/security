---
api_specs:
- filename: crescendo-lab-broadcast-api-openapi.yml
  format: yaml
  label: Crescendo Lab Broadcast API
  slug: crescendo-lab-broadcast-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-broadcast-api-openapi.yml
- filename: crescendo-lab-contacts-api-openapi.yml
  format: yaml
  label: Crescendo Lab Contacts API
  slug: crescendo-lab-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-contacts-api-openapi.yml
- filename: crescendo-lab-sms-api-openapi.yml
  format: yaml
  label: Crescendo Lab SMS API
  slug: crescendo-lab-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-sms-api-openapi.yml
- filename: crescendo-lab-teams-api-openapi.yml
  format: yaml
  label: Crescendo Lab Teams API
  slug: crescendo-lab-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-teams-api-openapi.yml
- filename: crescendo-lab-maac-go-api-api-openapi.yml
  format: yaml
  label: Crescendo Lab MAAC Go API
  slug: crescendo-lab-maac-go-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/openapi/crescendo-lab-maac-go-api-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cresclab.com
  spf: true
hosts:
- cert_expires: Sep 17 08:31:28 2026 GMT
  host: cresclab.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 04:51:15 2026 GMT
  host: sms.cresclab.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crescendo Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Crescendo Lab, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Crescendo Lab
provider_slug: crescendo-lab
slug: crescendo-lab-domain-security
source_filename: crescendo-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cresclab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 08:31:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sms.cresclab.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 04:51:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cresclab.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crescendo-lab/refs/heads/main/security/crescendo-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SMS
- Messaging
- Marketing Automation
- Customer Engagement
- Taiwan
- Omnichannel
- MCP
---
