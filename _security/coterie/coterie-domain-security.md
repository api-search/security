---
api_specs:
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Quotes API
  slug: coterie-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Policies API
  slug: coterie-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Applications API
  slug: coterie-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Industry / NAICS API
  slug: coterie-industry-naics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Documents API
  slug: coterie-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
- filename: coterie-openapi.yml
  format: yaml
  label: Coterie Webhooks API
  slug: coterie-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/openapi/coterie-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: coterieinsurance.com
  spf: true
hosts:
- cert_expires: Sep 12 17:26:19 2026 GMT
  host: coterieinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 07:43:19 2026 GMT
  host: docs.coterieinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  6 23:59:59 2026 GMT
  host: api.coterieinsurance.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coterie Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coterie Insurance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Coterie Insurance
provider_slug: coterie
slug: coterie-domain-security
source_filename: coterie-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coterieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 17:26:19 2026 GMT\n  hsts: false\n- host: docs.coterieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:43:19 2026 GMT\n  hsts: null\n- host: api.coterieinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: coterieinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coterie/refs/heads/main/security/coterie-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Insurance
- Commercial Insurance
- Small Business
- Embedded Insurance
- Insurtech
---
