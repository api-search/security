---
api_specs:
- filename: tcpcm-api-spec.yaml
  format: yaml
  label: Teamcenter Product Cost Management REST API
  slug: teamcenter-product-cost-management
  spec_type: OpenAPI
  url: https://developer.siemens.com/tcpcm/tcpcm-api-spec.yaml
- filename: polarion-rest-apispec.json
  format: json
  label: Polarion REST API
  slug: polarion-rest-api
  spec_type: OpenAPI
  url: https://developer.siemens.com/polarion/polarion-rest-apispec.json
- filename: product-information-api.spec.yaml
  format: yaml
  label: Product Information API
  slug: product-information-api
  spec_type: OpenAPI
  url: https://developer.siemens.com/product-information-api/product-information-api.spec.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: siemens.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: siemens.cloud
  spf: true
hosts:
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: www.plm.automation.siemens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: developer.siemens.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: product-information-hub.siemens.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Siemens Plm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Siemens PLM, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Siemens PLM
provider_slug: siemens-plm
slug: siemens-plm-domain-security
source_filename: siemens-plm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plm.automation.siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.siemens.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: product-information-hub.siemens.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: siemens.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: siemens.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/siemens-plm/refs/heads/main/security/siemens-plm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- PLM
- Product Lifecycle Management
- Teamcenter
- NX
- Solid Edge
- Simcenter
- Xcelerator
- Digital Manufacturing
- Industrial IoT
- CAD
- CAM
- Sustainability
- ALM
---
