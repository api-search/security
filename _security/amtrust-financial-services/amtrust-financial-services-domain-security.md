---
api_specs:
- filename: amtrust-financial-services-digital-wc-api-openapi.json
  format: json
  label: AmTrust Digital WC API
  slug: amtrust-financial-services-digital-wc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-wc-api-openapi.json
- filename: amtrust-financial-services-digital-bop-api-openapi.json
  format: json
  label: AmTrust Digital BOP API
  slug: amtrust-financial-services-digital-bop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-bop-api-openapi.json
- filename: amtrust-financial-services-digital-cyber-api-openapi.json
  format: json
  label: AmTrust Digital Cyber API
  slug: amtrust-financial-services-digital-cyber-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-cyber-api-openapi.json
- filename: amtrust-financial-services-digital-es-api-openapi.json
  format: json
  label: AmTrust Digital E&S API
  slug: amtrust-financial-services-digital-es-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-es-api-openapi.json
- filename: amtrust-financial-services-digital-pac-api-openapi.json
  format: json
  label: AmTrust Digital PAC API
  slug: amtrust-financial-services-digital-pac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-digital-pac-api-openapi.json
- filename: amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
  format: json
  label: AmTrust Reinsurance Contract Entry API
  slug: amtrust-financial-services-reinsurance-contract-entry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-reinsurance-contract-entry-api-openapi.json
- filename: amtrust-financial-services-experience-claims-medical-case-api-openapi.json
  format: json
  label: AmTrust Experience Claims Medical Case API
  slug: amtrust-financial-services-experience-claims-medical-case-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-experience-claims-medical-case-api-openapi.json
- filename: amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
  format: json
  label: AmTrust Experience Next Gen Bond Pro API
  slug: amtrust-financial-services-experience-next-gen-bond-pro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-experience-next-gen-bond-pro-api-openapi.json
- filename: amtrust-financial-services-conversa-engine-api-openapi.json
  format: json
  label: AmTrust Conversa Engine API
  slug: amtrust-financial-services-conversa-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/openapi/amtrust-financial-services-conversa-engine-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amtrustfinancial.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amtrustgroup.com
  spf: true
hosts:
- cert_expires: Oct 17 14:10:47 2026 GMT
  host: amtrustfinancial.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: apiportal.amtrustgroup.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: gateway.amtrustgroup.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amtrust Financial Services Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AmTrust Financial Services, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AmTrust Financial Services
provider_slug: amtrust-financial-services
slug: amtrust-financial-services-domain-security
source_filename: amtrust-financial-services-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amtrustfinancial.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 14:10:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: apiportal.amtrustgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.amtrustgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amtrustfinancial.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: amtrustgroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\nnotes:\n- 'apimanagement.amtrustgroup.com serves an EXPIRED wildcard certificate: subject CN=*.amtrustgroup.com,\n  O=AmTrust Financial Services, Inc., issued by Corporation Service Company RSA OV SSL CA, valid\
  \ 2023-11-28\n  to 2024-11-27 — expired roughly 21 months before this probe. It is the management endpoint that the\n  PRODUCTION developer portal at apiportal.amtrustgroup.com names in its own /config.json, so any browser\n  loading the production portal''s API list fails TLS validation. curl exits 60 (SSL certificate problem)\n  against it.'\n- prod-apim-gw.amtrustservices.com has no DNS record. It is the second servers[] entry in all nine published\n  production OpenAPI documents, so every AmTrust contract names an unreachable host.\n- gateway.amtrustgroup.com does not send Strict-Transport-Security on its root 404, but does send 'max-age=63072000;\n  includeSubDomains' on an authenticated-path 401 response.\nadditional_hosts:\n- host: apimanagement.amtrustgroup.com\n  https: false\n  tls_error: certificate expired 2024-11-27\n  cert_subject: C=US, ST=New York, O=AmTrust Financial Services, Inc., CN=*.amtrustgroup.com\n  cert_issuer: C=US, O=Corporation Service Company, CN=Corporation\
  \ Service Company RSA OV SSL CA\n  cert_not_before: '2023-11-28'\n  cert_not_after: '2024-11-27'\n- host: auth.amtrustgroup.com\n  https: true\n  note: OpenID Connect discovery served under /AuthServer\n- host: uatauth.amtrustgroup.com\n  https: true\n  note: UAT OpenID Connect discovery under /AuthServer_usertest\n- host: utapiportal.amtrustgroup.com\n  https: true\n  note: UAT Azure API Management developer portal\n- host: prod-apim-gw.amtrustservices.com\n  https: false\n  note: no DNS record\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amtrust-financial-services/refs/heads/main/security/amtrust-financial-services-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Insurance
- Insurance
- Property and Casualty
- Small Business
- Workers Compensation
- Fortune 1000
- Underwriting
- Claims
- Policy
- Reinsurance
- Cyber Insurance
- Surety
---
