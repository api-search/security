---
api_specs:
- filename: ozonetel-agent-api-openapi.yml
  format: yaml
  label: Ozonetel Agent API
  slug: ozonetel-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-agent-api-openapi.yml
- filename: ozonetel-aht-api-openapi.yml
  format: yaml
  label: Ozonetel AHT API
  slug: ozonetel-aht-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-aht-api-openapi.yml
- filename: ozonetel-campaign-api-openapi.yml
  format: yaml
  label: Ozonetel Campaign API
  slug: ozonetel-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-campaign-api-openapi.yml
- filename: ozonetel-campaign-reports-api-openapi.yml
  format: yaml
  label: Ozonetel Campaign Reports API
  slug: ozonetel-campaign-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-campaign-reports-api-openapi.yml
- filename: ozonetel-chat-campaign-api-openapi.yml
  format: yaml
  label: Ozonetel Chat Campaign API
  slug: ozonetel-chat-campaign-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-chat-campaign-api-openapi.yml
- filename: ozonetel-default-api-openapi.yml
  format: yaml
  label: Ozonetel Default API
  slug: ozonetel-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-default-api-openapi.yml
- filename: ozonetel-disposition-api-openapi.yml
  format: yaml
  label: Ozonetel Disposition API
  slug: ozonetel-disposition-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-disposition-api-openapi.yml
- filename: ozonetel-reports-api-openapi.yml
  format: yaml
  label: Ozonetel Reports API
  slug: ozonetel-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-reports-api-openapi.yml
- filename: ozonetel-sms-api-openapi.yml
  format: yaml
  label: Ozonetel SMS API
  slug: ozonetel-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ozonetel/openapi/ozonetel-sms-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ozonetel.com
  spf: true
hosts:
- cert_expires: Mar 28 23:59:59 2027 GMT
  host: ozonetel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ozonetel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ozonetel, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ozonetel
provider_slug: ozonetel
slug: ozonetel-domain-security
source_filename: ozonetel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ozonetel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 28 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ozonetel.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ozonetel/security/ozonetel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- CX Platform
- Cloud Communications
- Contact Center
- API
---
