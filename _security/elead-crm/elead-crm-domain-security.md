---
api_specs:
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Opportunities API
  slug: elead-crm-sales-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Customers API
  slug: elead-crm-sales-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Sales Activities API
  slug: elead-crm-sales-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
- filename: elead-crm-openapi.yml
  format: yaml
  label: Elead Product Reference Data API
  slug: elead-crm-product-reference-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/openapi/elead-crm-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eleadcrm.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fortellis.io
  spf: true
hosts:
- cert_expires: Sep 30 23:59:59 2026 GMT
  host: www.eleadcrm.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: apidocs.fortellis.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 23:59:59 2026 GMT
  host: api.fortellis.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Elead Crm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Elead, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Elead
provider_slug: elead-crm
slug: elead-crm-domain-security
source_filename: elead-crm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eleadcrm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 23:59:59 2026 GMT\n  hsts: false\n- host: apidocs.fortellis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.fortellis.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec  4 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: eleadcrm.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: fortellis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elead-crm/refs/heads/main/security/elead-crm-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- CRM
- Automotive
- Dealership
- Sales
- Leads
- Fortellis
- CDK Global
---
