---
api_specs:
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Inventory Items API
  slug: quartzy-inventory-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Order Requests API
  slug: quartzy-order-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Types API
  slug: quartzy-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Labs API
  slug: quartzy-labs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
- filename: quartzy-openapi.yml
  format: yaml
  label: Quartzy Webhooks API
  slug: quartzy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/openapi/quartzy-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: quartzy.com
  spf: true
hosts:
- cert_expires: Sep 12 06:52:43 2026 GMT
  host: www.quartzy.com
  hsts: true
  hsts_max_age: 3628800
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: docs.quartzy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: api.quartzy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quartzy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quartzy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Quartzy
provider_slug: quartzy
slug: quartzy-domain-security
source_filename: quartzy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quartzy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 06:52:43 2026 GMT\n  hsts: true\n  hsts_max_age: 3628800\n- host: docs.quartzy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: false\n- host: api.quartzy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: quartzy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quartzy/refs/heads/main/security/quartzy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Lab Management
- Inventory Management
- Life Sciences
- Procurement
- Ordering
- Laboratory
- Webhooks
---
