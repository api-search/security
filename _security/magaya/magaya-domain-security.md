---
api_specs:
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Shipments API
  slug: magaya-shipments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Warehouse Receipts API
  slug: magaya-warehouse-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Invoices API
  slug: magaya-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Items API
  slug: magaya-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
- filename: magaya-openapi.yml
  format: yaml
  label: Magaya Transactions API
  slug: magaya-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/openapi/magaya-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: magaya.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: magayacloud.com
  spf: true
hosts:
- cert_expires: Oct 21 14:46:03 2026 GMT
  host: www.magaya.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- host: systemid.magayacloud.com
  https: false
kind: domain-security
layout: security
method: probed
name: Magaya Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magaya, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Magaya
provider_slug: magaya
slug: magaya-domain-security
source_filename: magaya-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.magaya.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 21 14:46:03 2026 GMT\n  hsts: false\n- host: systemid.magayacloud.com\n  https: false\ndomains:\n- domain: magaya.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: magayacloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/magaya/refs/heads/main/security/magaya-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Logistics
- Supply Chain
- Freight Forwarding
- Warehouse Management
- Shipping
- Customs
- Transportation
---
