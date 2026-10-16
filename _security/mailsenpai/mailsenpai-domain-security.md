---
api_specs:
- filename: mailsenpai-account-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Account API
  slug: mailsenpai-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-account-api-openapi.yml
- filename: mailsenpai-log-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Log API
  slug: mailsenpai-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-log-api-openapi.yml
- filename: mailsenpai-sending-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Sending API
  slug: mailsenpai-sending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-sending-api-openapi.yml
- filename: mailsenpai-smtp-senpai-api-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) SMTP Senpai API
  slug: mailsenpai-smtp-senpai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-smtp-senpai-api-api-openapi.yml
- filename: mailsenpai-suppression-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Suppression API
  slug: mailsenpai-suppression-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-suppression-api-openapi.yml
- filename: mailsenpai-webhooks-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Webhooks API
  slug: mailsenpai-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-webhooks-api-openapi.yml
- filename: mailsenpai-website-forms-api-openapi.yml
  format: yaml
  label: SMTP Senpai (MailSenpai) Website forms API
  slug: mailsenpai-website-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/openapi/mailsenpai-website-forms-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailsenpai.com
  spf: true
hosts:
- cert_expires: Nov 28 12:31:16 2026 GMT
  host: en.mailsenpai.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailsenpai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SMTP Senpai (MailSenpai), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SMTP Senpai (MailSenpai)
provider_slug: mailsenpai
slug: mailsenpai-domain-security
source_filename: mailsenpai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.mailsenpai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 12:31:16 2026 GMT\n  hsts: false\ndomains:\n- domain: mailsenpai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailsenpai/refs/heads/main/security/mailsenpai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email marketing
- B2B outreach
- SMTP relay
- Artificial intelligence
- Newsletter platform
---
