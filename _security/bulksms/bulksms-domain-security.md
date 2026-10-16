---
api_specs:
- filename: bulksms-attachments-api-openapi.yml
  format: yaml
  label: BulkSMS Attachments API
  slug: bulksms-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-attachments-api-openapi.yml
- filename: bulksms-blocked-numbers-api-openapi.yml
  format: yaml
  label: BulkSMS Blocked Numbers API
  slug: bulksms-blocked-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-blocked-numbers-api-openapi.yml
- filename: bulksms-credits-api-openapi.yml
  format: yaml
  label: BulkSMS Credits API
  slug: bulksms-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-credits-api-openapi.yml
- filename: bulksms-message-api-openapi.yml
  format: yaml
  label: BulkSMS Message API
  slug: bulksms-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-message-api-openapi.yml
- filename: bulksms-profile-api-openapi.yml
  format: yaml
  label: BulkSMS Profile API
  slug: bulksms-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-profile-api-openapi.yml
- filename: bulksms-webhooks-api-openapi.yml
  format: yaml
  label: BulkSMS Webhooks API
  slug: bulksms-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bulksms.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: www.bulksms.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bulksms Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BulkSMS, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: BulkSMS
provider_slug: bulksms
slug: bulksms-domain-security
source_filename: bulksms-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bulksms.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: bulksms.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/security/bulksms-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- SMS
- Messaging
- Communications
- Business
- BulkSMS
---
