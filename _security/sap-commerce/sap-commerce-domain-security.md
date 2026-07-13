---
api_specs:
- filename: 66abfe678b55457fab235ce8039dda71.html
  format: yaml
  label: SAP Commerce Cloud OCC API
  slug: sap-commerce-occ-api
  spec_type: OpenAPI
  url: https://help.sap.com/docs/SAP_COMMERCE_CLOUD_PUBLIC_CLOUD/452dcbb0e00f47e88a69cdaeb87a925d/66abfe678b55457fab235ce8039dda71.html
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sap.com
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: www.sap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 25 23:59:59 2026 GMT
  host: help.sap.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.cloud.cx.sap.com
  https: false
kind: domain-security
layout: security
method: probed
name: Sap Commerce Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SAP Commerce Cloud, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SAP Commerce Cloud
provider_slug: sap-commerce
slug: sap-commerce-domain-security
source_filename: sap-commerce-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: null\n- host: help.sap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloud.cx.sap.com\n  https: false\ndomains:\n- domain: sap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-commerce/refs/heads/main/security/sap-commerce-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- E-Commerce
- Commerce
- Retail
- B2B
- B2C
- SAP
- Enterprise
- Omnichannel
- Products
- Orders
- Carts
---
