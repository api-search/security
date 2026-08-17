---
api_specs:
- filename: lucidya-ltd-social-listening-api-openapi.yml
  format: yaml
  label: Lucidya Social Listening API
  slug: lucidya-social-listening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-social-listening-api-openapi.yml
- filename: lucidya-ltd-ai-api-openapi.yml
  format: yaml
  label: Lucidya AI API
  slug: lucidya-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-ai-api-openapi.yml
- filename: lucidya-ltd-cdp-api-openapi.yml
  format: yaml
  label: Lucidya CDP API
  slug: lucidya-cdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-cdp-api-openapi.yml
- filename: lucidya-ltd-omnichannel-api-openapi.yml
  format: yaml
  label: Lucidya OmniChannel API
  slug: lucidya-omnichannel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-omnichannel-api-openapi.yml
- filename: lucidya-ltd-omniserve-analytics-api-openapi.yml
  format: yaml
  label: Lucidya OmniServe Analytics API
  slug: lucidya-omniserve-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/openapi/lucidya-ltd-omniserve-analytics-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lucidya.com
  spf: true
hosts:
- cert_expires: Oct 13 06:11:11 2026 GMT
  host: lucidya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 03:46:11 2026 GMT
  host: docs.lucidya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 12 04:39:13 2026 GMT
  host: api.lucidya.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lucidya Ltd Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lucidya Ltd, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Lucidya Ltd
provider_slug: lucidya-ltd
slug: lucidya-ltd-domain-security
source_filename: lucidya-ltd-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lucidya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 06:11:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.lucidya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 03:46:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.lucidya.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:39:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lucidya.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucidya-ltd/refs/heads/main/security/lucidya-ltd-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Customer Experience
- Social Listening
- Customer Data Platform
- Analytics
- Artificial Intelligence
- Omnichannel
- Arabic NLP
- MENA
---
