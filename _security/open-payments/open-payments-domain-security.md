---
api_specs:
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments General Payments API
  slug: open-payments-general-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Research Payments API
  slug: open-payments-research-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Ownership and Investment API
  slug: open-payments-ownership-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Datastore Query API
  slug: open-payments-datastore-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
- filename: open-payments-openapi.yml
  format: yaml
  label: Open Payments Metastore and Search API
  slug: open-payments-metastore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/openapi/open-payments-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_policy: reject
  domain: cms.gov
  notes: Federal .gov domain. DMARC is enforced with p=reject and DHS Cyber aggregate/forensic reporting. Served over TLS 1.3 with HSTS (max-age 31536000, includeSubDomains).
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  cipher: TLS_AES_256_GCM_SHA384
  host: openpaymentsdata.cms.gov
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Payments Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CMS Open Payments, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: CMS Open Payments
provider_slug: open-payments
slug: open-payments-domain-security
source_filename: open-payments-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openpaymentsdata.cms.gov\n  https: true\n  tls_version: TLSv1.3\n  cipher: TLS_AES_256_GCM_SHA384\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: cms.gov\n  dmarc: true\n  dmarc_policy: reject\n  notes: >-\n    Federal .gov domain. DMARC is enforced with p=reject and DHS Cyber\n    aggregate/forensic reporting. Served over TLS 1.3 with HSTS\n    (max-age 31536000, includeSubDomains).\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-payments/refs/heads/main/security/open-payments-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government Data
- Healthcare
- Open Data
- Transparency
- Payments
- Clinical Data
- Physicians
- Open Government
- Public Sector
---
