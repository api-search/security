---
api_specs:
- filename: celigo-webhook-listeners-asyncapi.yml
  format: yaml
  label: Celigo integrator.io Webhook Listeners
  slug: celigo-webhook-listeners
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/asyncapi/celigo-webhook-listeners-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:security@celigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: celigo.com
  spf: true
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: integrator.io
  spf: true
hosts:
- cert_expires: Aug 29 15:28:45 2026 GMT
  host: celigo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 23:40:49 2026 GMT
  host: docs.celigo.com
  hsts: true
  hsts_max_age: 259200
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 30 23:59:59 2026 GMT
  host: api.integrator.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Celigo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Celigo, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Celigo
provider_slug: celigo
slug: celigo-domain-security
source_filename: celigo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: celigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 15:28:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.celigo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 23:40:49 2026 GMT\n  hsts: true\n  hsts_max_age: 259200\n- host: api.integrator.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: celigo.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:security@celigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: integrator.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/celigo/refs/heads/main/security/celigo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- API Management
- Automation
- Data Integration
- Integration
- iPaaS
- Workflow
---
