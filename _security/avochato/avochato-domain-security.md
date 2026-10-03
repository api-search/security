---
api_specs:
- filename: avochato-avochato-api-api-openapi.yml
  format: yaml
  label: Avochato Avochato API
  slug: avochato-avochato-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-avochato-api-api-openapi.yml
- filename: avochato-broadcasts-api-openapi.yml
  format: yaml
  label: Avochato Broadcasts API
  slug: avochato-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-broadcasts-api-openapi.yml
- filename: avochato-campaigns-api-openapi.yml
  format: yaml
  label: Avochato Campaigns API
  slug: avochato-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-campaigns-api-openapi.yml
- filename: avochato-contacts-api-openapi.yml
  format: yaml
  label: Avochato Contacts API
  slug: avochato-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-contacts-api-openapi.yml
- filename: avochato-links-api-openapi.yml
  format: yaml
  label: Avochato Links API
  slug: avochato-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-links-api-openapi.yml
- filename: avochato-messages-api-openapi.yml
  format: yaml
  label: Avochato Messages API
  slug: avochato-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-messages-api-openapi.yml
- filename: avochato-tickets-api-openapi.yml
  format: yaml
  label: Avochato Tickets API
  slug: avochato-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/openapi/avochato-tickets-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazonaws.com"
  - 0 iodef "mailto:ops@avochato.com"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: avochato.com
  spf: true
hosts:
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: www.avochato.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Avochato Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Avochato, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Avochato
provider_slug: avochato
slug: avochato-domain-security
source_filename: avochato-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.avochato.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: avochato.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 iodef \"mailto:ops@avochato.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avochato/refs/heads/main/security/avochato-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Messaging
- SMS
- RCS
- Voice
- Business
---
