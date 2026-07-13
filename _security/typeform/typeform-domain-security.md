---
api_specs:
- filename: typeform-openapi.yml
  format: yaml
  label: Typeform Create API
  slug: create
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeform/refs/heads/main/openapi/typeform-openapi.yml
- filename: typeform-asyncapi.yml
  format: yaml
  label: Typeform Webhooks API
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/typeform/refs/heads/main/asyncapi/typeform-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:security@typeform.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: typeform.com
  spf: true
hosts:
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: www.typeform.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: api.typeform.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 29 23:59:59 2026 GMT
  host: embed.typeform.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Typeform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Typeform, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Typeform
provider_slug: typeform
slug: typeform-domain-security
source_filename: typeform-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.typeform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: api.typeform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: null\n- host: embed.typeform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: typeform.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:security@typeform.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/typeform/refs/heads/main/security/typeform-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Forms
- Surveys
- Conversational
- Lead Capture
- SaaS
- Webhooks
- Embed
---
