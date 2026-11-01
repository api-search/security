---
api_specs:
- filename: sugarcrm-com-rest-api-openapi.yml
  format: yaml
  label: SugarCRM REST API
  slug: sugarcrm-rest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sugarcrm-com/openapi/sugarcrm-com-rest-api-openapi.yml
- filename: sugarcrm-com-openapi-generated.yml
  format: yaml
  label: SugarCRM API
  slug: sugarcrm-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sugarcrm-com/openapi/_ae-authored/sugarcrm-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sugarcrm.com
  spf: true
hosts:
- cert_expires: Dec  2 00:41:21 2026 GMT
  host: www.sugarcrm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sugarcrm Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SugarCRM, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SugarCRM
provider_slug: sugarcrm-com
slug: sugarcrm-com-domain-security
source_filename: sugarcrm-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sugarcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 00:41:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: sugarcrm.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/sugarcrm-com/security/sugarcrm-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CRM
- Sales
- B2B
- SaaS
- AI
- Integration
---
