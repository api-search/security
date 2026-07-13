---
api_specs:
- filename: expedia-rapid-openapi-original.yml
  format: yaml
  label: Expedia Rapid API
  slug: rapid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-rapid-openapi-original.yml
- filename: expedia-fraud-protection-openapi-original.yml
  format: yaml
  label: Expedia Fraud Protection API
  slug: fraud-protection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-fraud-protection-openapi-original.yml
- filename: expedia-lodging-product-openapi-original.yml
  format: yaml
  label: Expedia Lodging API
  slug: lodging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-lodging-product-openapi-original.yml
- filename: expedia-deposit-openapi-original.yml
  format: yaml
  label: Expedia EPS Deposit API
  slug: deposit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-deposit-openapi-original.yml
- filename: expedia-loyalty-openapi-original.yml
  format: yaml
  label: Expedia Loyalty Earn API
  slug: loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-loyalty-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: expediagroup.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: expediaconnectivity.com
  spf: false
hosts:
- cert_expires: Aug 27 15:29:40 2026 GMT
  host: developers.expediagroup.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 10:06:17 2026 GMT
  host: expediaconnectivity.com
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: services.expediapartnercentral.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Expedia Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Expedia Group, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Expedia Group
provider_slug: expedia-group
slug: expedia-group-domain-security
source_filename: expedia-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.expediagroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:29:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: expediaconnectivity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 10:06:17 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: services.expediapartnercentral.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: expediagroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: expediaconnectivity.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/security/expedia-group-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Flights
- Hotels
- Lodging
- Travel
- Fortune 500
---
