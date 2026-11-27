---
api_specs:
- filename: billboardbug-com-ai-api-openapi.yml
  format: yaml
  label: BillboardBug AI API
  slug: billboardbug-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-ai-api-openapi.yml
- filename: billboardbug-com-blob-api-openapi.yml
  format: yaml
  label: BillboardBug Blob API
  slug: billboardbug-com-blob-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-blob-api-openapi.yml
- filename: billboardbug-com-business-api-openapi.yml
  format: yaml
  label: BillboardBug Business API
  slug: billboardbug-com-business-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-business-api-openapi.yml
- filename: billboardbug-com-globalconfig-api-openapi.yml
  format: yaml
  label: BillboardBug Global Config API
  slug: billboardbug-com-globalconfig-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-globalconfig-api-openapi.yml
- filename: billboardbug-com-post-api-openapi.yml
  format: yaml
  label: BillboardBug Post API
  slug: billboardbug-com-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/billboardbug-com/openapi/billboardbug-com-post-api-openapi.yml
description: ''
domains:
- caa:
  - agreeable-field-0c278c00f.1.azurestaticapps.net.
  - azurestaticapps1.trafficmanager.net.
  - msha-slice-1-eus2-1.msha-slice-1-eus2-1-ase.p.azurewebsites.net.
  - waws-prod-bn1-36496307.sip.p.azurewebsites.windows.net.
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: billboardbug.com
  spf: false
hosts:
- cert_expires: May  1 23:59:59 2027 GMT
  host: billboardbug.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BillboardBug Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BillboardBug, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=none).'
provider_name: BillboardBug
provider_slug: billboardbug-com
slug: billboardbug-com-domain-security
source_filename: billboardbug-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: billboardbug.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: billboardbug.com\n  dnssec: true\n  caa:\n  - agreeable-field-0c278c00f.1.azurestaticapps.net.\n  - azurestaticapps1.trafficmanager.net.\n  - msha-slice-1-eus2-1.msha-slice-1-eus2-1-ase.p.azurewebsites.net.\n  - waws-prod-bn1-36496307.sip.p.azurewebsites.windows.net.\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/billboardbug-com/security/billboardbug-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Advertising
- Local Business
- Mobile App
- Small Business
---
