---
api_specs:
- filename: soldo-software-and-services-business-api-openapi.json
  format: json
  label: Soldo Business API
  slug: soldo-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/soldo-software-and-services/refs/heads/main/openapi/soldo-software-and-services-business-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: soldo.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: soldocloud.net
  spf: false
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: api.soldo.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 12 23:59:59 2027 GMT
  host: api-demo.soldocloud.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Soldo Software And Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Soldo Software and Services, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Soldo Software and Services
provider_slug: soldo-software-and-services
slug: soldo-software-and-services-domain-security
source_filename: soldo-software-and-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.soldo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: null\n- host: api-demo.soldocloud.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: soldo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: soldocloud.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soldo-software-and-services/refs/heads/main/security/soldo-software-and-services-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Spend Management
- Expense Management
- Payments
- Business Cards
- Prepaid Cards
- Fintech
- Financial Services
- Webhooks
---
