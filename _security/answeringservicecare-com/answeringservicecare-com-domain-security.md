---
api_specs:
- filename: answeringservicecare-com-batch-api-openapi.yml
  format: yaml
  label: answeringservicecare-com Batch API
  slug: answeringservicecare-com-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answeringservicecare-com/openapi/answeringservicecare-com-batch-api-openapi.yml
- filename: answeringservicecare-com-company-api-openapi.yml
  format: yaml
  label: answeringservicecare-com Company API
  slug: answeringservicecare-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answeringservicecare-com/openapi/answeringservicecare-com-company-api-openapi.yml
- filename: answeringservicecare-com-content-api-openapi.yml
  format: yaml
  label: answeringservicecare-com Content API
  slug: answeringservicecare-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answeringservicecare-com/openapi/answeringservicecare-com-content-api-openapi.yml
- filename: answeringservicecare-com-offerings-api-openapi.yml
  format: yaml
  label: answeringservicecare-com Offerings API
  slug: answeringservicecare-com-offerings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answeringservicecare-com/openapi/answeringservicecare-com-offerings-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: answeringservicecare.com
  spf: true
hosts:
- cert_expires: Jan 17 19:59:20 2027 GMT
  host: answeringservicecare.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Answeringservicecare Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for answeringservicecare-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: answeringservicecare-com
provider_slug: answeringservicecare-com
slug: answeringservicecare-com-domain-security
source_filename: answeringservicecare-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: answeringservicecare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:59:20 2027 GMT\n  hsts: null\ndomains:\n- domain: answeringservicecare.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/answeringservicecare-com/security/answeringservicecare-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Telephony
- Call Center
- VirtualAnswering
- Customer Service
- Communications
---
