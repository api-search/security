---
api_specs:
- filename: diebold-dn-open-backend-api-openapi.yml
  format: yaml
  label: DN Open Backend API
  slug: dn-open-backend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-open-backend-api-openapi.yml
- filename: diebold-dn-online-mobile-api-openapi.yml
  format: yaml
  label: DN Online & Mobile API
  slug: dn-online-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-online-mobile-api-openapi.yml
- filename: diebold-dn-assist-api-openapi.yml
  format: yaml
  label: DN Assist API
  slug: dn-assist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-assist-api-openapi.yml
- filename: diebold-dn-payment-initiation-api-openapi.yml
  format: yaml
  label: DN Payment Initiation API
  slug: dn-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-payment-initiation-api-openapi.yml
- filename: diebold-dn-tm-authorization-api-openapi.yml
  format: yaml
  label: DN TM Authorization API
  slug: dn-tm-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-tm-authorization-api-openapi.yml
- filename: diebold-dn-account-bc-api-openapi.yml
  format: yaml
  label: DN Account BC API
  slug: dn-account-bc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-account-bc-api-openapi.yml
- filename: diebold-dn-secure-business-processing-api-openapi.yml
  format: yaml
  label: DN Secure Business Processing API
  slug: dn-secure-business-processing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-dn-secure-business-processing-api-openapi.yml
- filename: diebold-tm-pre-digitization-api-outbound-openapi.yml
  format: yaml
  label: TM Pre-Digitization API (Outbound)
  slug: tm-pre-digitization-api-outbound
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/openapi/diebold-tm-pre-digitization-api-outbound-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: dieboldnixdorf.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: swaggerhub.com
  spf: true
hosts:
- cert_expires: Jan 30 23:59:59 2027 GMT
  host: www.dieboldnixdorf.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 13:07:03 2026 GMT
  host: vrp-api.dieboldnixdorf.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 14 23:59:59 2026 GMT
  host: virtserver.swaggerhub.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Diebold Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diebold Nixdorf, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Diebold Nixdorf
provider_slug: diebold
slug: diebold-domain-security
source_filename: diebold-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dieboldnixdorf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  hsts: null\n- host: vrp-api.dieboldnixdorf.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 13:07:03 2026 GMT\n  hsts: false\n- host: virtserver.swaggerhub.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dieboldnixdorf.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: swaggerhub.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diebold/refs/heads/main/security/diebold-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Banking
- Retail
- ATM
- Self-Service
- Point-of-Sale
- Payments
- Transaction Middleware
- Vynamic
- Open Banking
- Fortune 1000
---
