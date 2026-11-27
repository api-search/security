---
api_specs:
- filename: mailfornet-com-account-api-openapi.yml
  format: yaml
  label: Mailfornet Account API
  slug: mailfornet-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-account-api-openapi.yml
- filename: mailfornet-com-inboxes-api-openapi.yml
  format: yaml
  label: Mailfornet Inboxes API
  slug: mailfornet-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-inboxes-api-openapi.yml
- filename: mailfornet-com-messages-api-openapi.yml
  format: yaml
  label: Mailfornet Messages API
  slug: mailfornet-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-messages-api-openapi.yml
- filename: mailfornet-com-webhooks-api-openapi.yml
  format: yaml
  label: Mailfornet Webhooks API
  slug: mailfornet-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfornet-com/openapi/mailfornet-com-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mailfornet.com
  spf: true
hosts:
- cert_expires: Feb 12 19:52:09 2027 GMT
  host: mailfornet.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mailfornet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailfornet, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mailfornet
provider_slug: mailfornet-com
slug: mailfornet-com-domain-security
source_filename: mailfornet-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailfornet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 12 19:52:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: mailfornet.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mailfornet-com/security/mailfornet-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- temporary-email
- Disposable Email
- Email Verification
- Privacy
- Developer API
---
