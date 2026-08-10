---
api_specs:
- filename: autoleadstar-activities-api-openapi.yml
  format: yaml
  label: AutoLeadStar Activities API
  slug: autoleadstar-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-activities-api-openapi.yml
- filename: autoleadstar-appointments-api-openapi.yml
  format: yaml
  label: AutoLeadStar Appointments API
  slug: autoleadstar-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-appointments-api-openapi.yml
- filename: autoleadstar-audiences-api-openapi.yml
  format: yaml
  label: AutoLeadStar Audiences API
  slug: autoleadstar-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-audiences-api-openapi.yml
- filename: autoleadstar-consents-api-openapi.yml
  format: yaml
  label: AutoLeadStar Consents API
  slug: autoleadstar-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-consents-api-openapi.yml
- filename: autoleadstar-leads-api-openapi.yml
  format: yaml
  label: AutoLeadStar Leads API
  slug: autoleadstar-leads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-leads-api-openapi.yml
- filename: autoleadstar-shoppers-api-openapi.yml
  format: yaml
  label: AutoLeadStar Shoppers API
  slug: autoleadstar-shoppers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-shoppers-api-openapi.yml
- filename: autoleadstar-tasks-api-openapi.yml
  format: yaml
  label: AutoLeadStar Tasks API
  slug: autoleadstar-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/openapi/autoleadstar-tasks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fullpath.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forgeglobal.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.fullpath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 20:15:48 2026 GMT
  host: forgeglobal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 19 23:59:59 2027 GMT
  host: developers.fullpath.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autoleadstar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AutoLeadStar, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AutoLeadStar
provider_slug: autoleadstar
slug: autoleadstar-domain-security
source_filename: autoleadstar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fullpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: false\n- host: forgeglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 20:15:48 2026 GMT\n  hsts: null\n- host: developers.fullpath.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: fullpath.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: forgeglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autoleadstar/refs/heads/main/security/autoleadstar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Automotive
- Customer Data Platform
- Marketing Automation
- Dealerships
- Advertising
- Artificial Intelligence
- Consent Management
- CRM
- Israel
---
