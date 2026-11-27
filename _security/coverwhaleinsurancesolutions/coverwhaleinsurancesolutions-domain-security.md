---
api_specs:
- filename: coverwhaleinsurancesolutions-authentication-api-openapi.yml
  format: yaml
  label: Cover Whale Authentication API
  slug: coverwhaleinsurancesolutions-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-authentication-api-openapi.yml
- filename: coverwhaleinsurancesolutions-binding-api-openapi.yml
  format: yaml
  label: Cover Whale Binding API
  slug: coverwhaleinsurancesolutions-binding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-binding-api-openapi.yml
- filename: coverwhaleinsurancesolutions-policy-lifecycle-api-openapi.yml
  format: yaml
  label: Cover Whale Policy Lifecycle API
  slug: coverwhaleinsurancesolutions-policy-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-policy-lifecycle-api-openapi.yml
- filename: coverwhaleinsurancesolutions-quoting-api-openapi.yml
  format: yaml
  label: Cover Whale Quoting API
  slug: coverwhaleinsurancesolutions-quoting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-quoting-api-openapi.yml
- filename: coverwhaleinsurancesolutions-reference-data-api-openapi.yml
  format: yaml
  label: Cover Whale Reference Data API
  slug: coverwhaleinsurancesolutions-reference-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-reference-data-api-openapi.yml
- filename: coverwhaleinsurancesolutions-submission-data-api-openapi.yml
  format: yaml
  label: Cover Whale Submission Data API
  slug: coverwhaleinsurancesolutions-submission-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-submission-data-api-openapi.yml
- filename: coverwhaleinsurancesolutions-submissions-api-openapi.yml
  format: yaml
  label: Cover Whale Submissions API
  slug: coverwhaleinsurancesolutions-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-submissions-api-openapi.yml
- filename: coverwhaleinsurancesolutions-webhooks-api-openapi.yml
  format: yaml
  label: Cover Whale Webhooks API
  slug: coverwhaleinsurancesolutions-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coverwhaleinsurancesolutions/openapi/coverwhaleinsurancesolutions-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: coverwhale.com
  spf: true
hosts:
- cert_expires: Dec 23 00:15:33 2026 GMT
  host: coverwhale.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cover Whale Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cover Whale, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Cover Whale
provider_slug: coverwhaleinsurancesolutions
slug: coverwhaleinsurancesolutions-domain-security
source_filename: coverwhaleinsurancesolutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coverwhale.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 00:15:33 2026 GMT\n  hsts: false\ndomains:\n- domain: coverwhale.com\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/coverwhaleinsurancesolutions/security/coverwhaleinsurancesolutions-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Insurance
- Commercial Auto Insurance
- Insurtech
- Underwriting
- Telematics
- Risk Management
- Fleet Safety
- Policy Lifecycle
- Webhook
- Company
---
