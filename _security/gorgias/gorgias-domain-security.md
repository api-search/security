---
api_specs:
- filename: gorgias-openapi.yml
  format: yaml
  label: Gorgias REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-openapi.yml
- filename: gorgias-asyncapi.yml
  format: yaml
  label: Gorgias Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/asyncapi/gorgias-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gorgias.com
  spf: true
hosts:
- cert_expires: Sep 19 16:43:39 2026 GMT
  host: www.gorgias.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 19:15:48 2026 GMT
  host: developers.gorgias.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gorgias Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gorgias, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gorgias
provider_slug: gorgias
slug: gorgias-domain-security
source_filename: gorgias-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gorgias.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 16:43:39 2026 GMT\n  hsts: false\n- host: developers.gorgias.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 19:15:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gorgias.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/security/gorgias-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Support
- Helpdesk
- Ecommerce
- Shopify
- Tickets
- Conversations
---
