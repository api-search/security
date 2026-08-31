---
api_specs:
- filename: barogo-areas-api-openapi.yml
  format: yaml
  label: Barogo Areas API
  slug: barogo-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-areas-api-openapi.yml
- filename: barogo-delivery-api-openapi.yml
  format: yaml
  label: Barogo Delivery API
  slug: barogo-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-delivery-api-openapi.yml
- filename: barogo-deposits-api-openapi.yml
  format: yaml
  label: Barogo Deposits API
  slug: barogo-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-deposits-api-openapi.yml
- filename: barogo-orders-api-openapi.yml
  format: yaml
  label: Barogo Orders API
  slug: barogo-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-orders-api-openapi.yml
- filename: barogo-stores-api-openapi.yml
  format: yaml
  label: Barogo Stores API
  slug: barogo-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/openapi/barogo-stores-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: barogo.com
  spf: true
  spf_record: v=spf1 ip4:18.168.51.200 ip4:18.168.140.58 include:mail.stibee.com include:spf.protection.outlook.com include:amazonses.com ~all
- caa: []
  dmarc: false
  dmarc_policy: null
  dnssec: false
  domain: gorelas.com
  spf: false
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.barogo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: developer.gorelas.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api-interlocker.gorelas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: staging-api-interlocker.gorelas.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Barogo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Barogo, probed live across 4 host(s) and 2 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Barogo
provider_slug: barogo
slug: barogo-domain-security
source_filename: barogo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.barogo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: false\n- host: developer.gorelas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: false\n- host: api-interlocker.gorelas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: staging-api-interlocker.gorelas.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: barogo.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 ip4:18.168.51.200 ip4:18.168.140.58 include:mail.stibee.com include:spf.protection.outlook.com\n    include:amazonses.com ~all\n  dmarc: false\n  dmarc_policy: null\n- domain: gorelas.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dmarc_policy: null\n\
  findings:\n- No HSTS on any host, including the production API host and the developer portal.\n- No CAA record on either domain, so certificate issuance is unconstrained.\n- No DNSSEC on either domain.\n- barogo.com publishes SPF but no DMARC record, so there is no policy on spoofed mail from the\n  brand domain. gorelas.com — the domain that carries the API, the developer portal and the\n  admin consoles — publishes neither SPF nor DMARC.\n- TLS 1.3 with valid certificates everywhere probed. That part is clean.\ncorrections:\n- field: barogo.com dnssec / caa\n  detail: >-\n    An automated pass initially recorded dnssec:true and a CAA value of\n    \"production-homepage-lb-2000987377.ap-northeast-2.elb.amazonaws.com.\" for barogo.com. That\n    is wrong. barogo.com is a CNAME at the apex pointing at an AWS ELB, so `dig DNSKEY` and\n    `dig CAA` both follow the CNAME and echo the target hostname. Re-verified directly: no\n    DNSKEY, no CAA record. Corrected to false / [].\n  corrected:\
  \ '2026-08-06'\nx-evidence:\n  fetched: '2026-08-06'\n  method: dig + TLS handshake + HTTP HEAD\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barogo/refs/heads/main/security/barogo-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Delivery
- Logistics
- Last Mile Delivery
- Food Delivery
- Courier
- Fulfillment
- Order
- Webhook
- South Korea
- Transportation
- Marketplace
---
