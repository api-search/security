---
api_specs:
- filename: smtp2go-email-api-openapi.yml
  format: yaml
  label: SMTP2GO Email API
  slug: smtp2go-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-email-api-openapi.yml
- filename: smtp2go-activity-api-openapi.yml
  format: yaml
  label: SMTP2GO Activity API
  slug: smtp2go-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-activity-api-openapi.yml
- filename: smtp2go-api-keys-api-openapi.yml
  format: yaml
  label: SMTP2GO API Keys API
  slug: smtp2go-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-api-keys-api-openapi.yml
- filename: smtp2go-domains-api-openapi.yml
  format: yaml
  label: SMTP2GO Domains API
  slug: smtp2go-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-domains-api-openapi.yml
- filename: smtp2go-sms-api-openapi.yml
  format: yaml
  label: SMTP2GO SMS API
  slug: smtp2go-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-sms-api-openapi.yml
- filename: smtp2go-smtp-users-api-openapi.yml
  format: yaml
  label: SMTP2GO SMTP Users API
  slug: smtp2go-smtp-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-smtp-users-api-openapi.yml
- filename: smtp2go-stats-api-openapi.yml
  format: yaml
  label: SMTP2GO Stats API
  slug: smtp2go-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-stats-api-openapi.yml
- filename: smtp2go-subaccounts-api-openapi.yml
  format: yaml
  label: SMTP2GO Subaccounts API
  slug: smtp2go-subaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-subaccounts-api-openapi.yml
- filename: smtp2go-suppressions-api-openapi.yml
  format: yaml
  label: SMTP2GO Suppressions API
  slug: smtp2go-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-suppressions-api-openapi.yml
- filename: smtp2go-templates-api-openapi.yml
  format: yaml
  label: SMTP2GO Templates API
  slug: smtp2go-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-templates-api-openapi.yml
- filename: smtp2go-webhooks-api-openapi.yml
  format: yaml
  label: SMTP2GO Webhooks API
  slug: smtp2go-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: smtp2go.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: www.smtp2go.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:02:51 2026 GMT
  host: developers.smtp2go.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.smtp2go.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smtp2Go Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMTP2GO, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SMTP2GO
provider_slug: smtp2go
slug: smtp2go-domain-security
source_filename: smtp2go-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smtp2go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: developers.smtp2go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:02:51 2026 GMT\n  hsts: null\n- host: api.smtp2go.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: smtp2go.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/security/smtp2go-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Email Delivery
- Transactional Email
- SMTP
- SMS
- Email API
- Deliverability
---
