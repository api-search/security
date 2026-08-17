---
api_specs:
- filename: mailersend-bulk-email-api-openapi.yml
  format: yaml
  label: MailerSend Bulk Email API
  slug: mailersend-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-bulk-email-api-openapi.yml
- filename: mailersend-domains-api-openapi.yml
  format: yaml
  label: MailerSend Domains API
  slug: mailersend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-domains-api-openapi.yml
- filename: mailersend-email-api-openapi.yml
  format: yaml
  label: MailerSend Email API
  slug: mailersend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-email-api-openapi.yml
- filename: mailersend-messages-api-openapi.yml
  format: yaml
  label: MailerSend Messages API
  slug: mailersend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-messages-api-openapi.yml
- filename: mailersend-sender-identities-api-openapi.yml
  format: yaml
  label: MailerSend Sender Identities API
  slug: mailersend-sender-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-sender-identities-api-openapi.yml
- filename: mailersend-templates-api-openapi.yml
  format: yaml
  label: MailerSend Templates API
  slug: mailersend-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-templates-api-openapi.yml
- filename: mailersend-webhooks-api-openapi.yml
  format: yaml
  label: MailerSend Webhooks API
  slug: mailersend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailersend.com
  spf: true
hosts:
- cert_expires: Sep 15 10:10:15 2026 GMT
  host: www.mailersend.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 28 12:31:44 2026 GMT
  host: developers.mailersend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 10:10:15 2026 GMT
  host: api.mailersend.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailersend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailerSend, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MailerSend
provider_slug: mailersend
slug: mailersend-domain-security
source_filename: mailersend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailersend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:10:15 2026 GMT\n  hsts: null\n- host: developers.mailersend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 12:31:44 2026 GMT\n  hsts: false\n- host: api.mailersend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 10:10:15 2026 GMT\n  hsts: false\ndomains:\n- domain: mailersend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/security/mailersend-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Transactional Email
- SMTP
- Marketing
- Communications
- SMS
- Messaging
- Templates
- Webhooks
- Email Verification
- Deliverability
- Analytics
- MCP
---
