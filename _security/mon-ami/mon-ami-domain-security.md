---
api_specs:
- filename: mon-ami-care-plans-api-openapi.yml
  format: yaml
  label: Mon Ami Care Plans API
  slug: mon-ami-care-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-care-plans-api-openapi.yml
- filename: mon-ami-client-calls-api-openapi.yml
  format: yaml
  label: Mon Ami Client Calls API
  slug: mon-ami-client-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-client-calls-api-openapi.yml
- filename: mon-ami-clients-api-openapi.yml
  format: yaml
  label: Mon Ami Clients API
  slug: mon-ami-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-clients-api-openapi.yml
- filename: mon-ami-copays-api-openapi.yml
  format: yaml
  label: Mon Ami Copays API
  slug: mon-ami-copays-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-copays-api-openapi.yml
- filename: mon-ami-documents-api-openapi.yml
  format: yaml
  label: Mon Ami Documents API
  slug: mon-ami-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-documents-api-openapi.yml
- filename: mon-ami-funding-sources-api-openapi.yml
  format: yaml
  label: Mon Ami Funding Sources API
  slug: mon-ami-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-funding-sources-api-openapi.yml
- filename: mon-ami-languages-api-openapi.yml
  format: yaml
  label: Mon Ami Languages API
  slug: mon-ami-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-languages-api-openapi.yml
- filename: mon-ami-people-api-openapi.yml
  format: yaml
  label: Mon Ami People API
  slug: mon-ami-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-people-api-openapi.yml
- filename: mon-ami-programs-api-openapi.yml
  format: yaml
  label: Mon Ami Programs API
  slug: mon-ami-programs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-programs-api-openapi.yml
- filename: mon-ami-provider-referrals-api-openapi.yml
  format: yaml
  label: Mon Ami Provider Referrals API
  slug: mon-ami-provider-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-provider-referrals-api-openapi.yml
- filename: mon-ami-providers-api-openapi.yml
  format: yaml
  label: Mon Ami Providers API
  slug: mon-ami-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-providers-api-openapi.yml
- filename: mon-ami-services-api-openapi.yml
  format: yaml
  label: Mon Ami Services API
  slug: mon-ami-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-services-api-openapi.yml
- filename: mon-ami-sites-api-openapi.yml
  format: yaml
  label: Mon Ami Sites API
  slug: mon-ami-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-sites-api-openapi.yml
- filename: mon-ami-tasks-api-openapi.yml
  format: yaml
  label: Mon Ami Tasks API
  slug: mon-ami-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-tasks-api-openapi.yml
- filename: mon-ami-visits-api-openapi.yml
  format: yaml
  label: Mon Ami Visits API
  slug: mon-ami-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-visits-api-openapi.yml
- filename: mon-ami-volunteers-api-openapi.yml
  format: yaml
  label: Mon Ami Volunteers API
  slug: mon-ami-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-volunteers-api-openapi.yml
- filename: mon-ami-webhooks-api-openapi.yml
  format: yaml
  label: Mon Ami Webhooks API
  slug: mon-ami-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/openapi/mon-ami-webhooks-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:admin@monami.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monami.io
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: www.monami.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mon Ami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mon Ami, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mon Ami
provider_slug: mon-ami
slug: mon-ami-domain-security
source_filename: mon-ami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.monami.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: monami.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:admin@monami.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mon-ami/refs/heads/main/security/mon-ami-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Aging Services
- Disability Services
- Case Management
- Care Coordination
- HL7 FHIR
- HIPAA
---
