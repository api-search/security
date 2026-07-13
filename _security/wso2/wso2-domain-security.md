---
api_specs:
- filename: wso2-publisher-api.yaml
  format: yaml
  label: WSO2 Publisher API
  slug: publisher-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-publisher-api.yaml
- filename: wso2-devportal-api.yaml
  format: yaml
  label: WSO2 Developer Portal API
  slug: devportal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-devportal-api.yaml
- filename: wso2-admin-api.yaml
  format: yaml
  label: WSO2 Admin Portal API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-admin-api.yaml
- filename: wso2-gateway-api.yaml
  format: yaml
  label: WSO2 Gateway API
  slug: gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-gateway-api.yaml
- filename: wso2-service-catalog-api.yaml
  format: yaml
  label: WSO2 Service Catalog API
  slug: service-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-service-catalog-api.yaml
- filename: wso2-devops-api.yaml
  format: yaml
  label: WSO2 DevOps API
  slug: devops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-devops-api.yaml
- filename: wso2-dcr-api.yaml
  format: yaml
  label: WSO2 DCR API
  slug: dcr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-dcr-api.yaml
- filename: wso2-governance-api.yaml
  format: yaml
  label: WSO2 Governance API
  slug: governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/openapi/wso2-governance-api.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: wso2.com
  spf: true
hosts:
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: wso2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 04:29:12 2026 GMT
  host: apim.docs.wso2.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 21 23:59:59 2026 GMT
  host: apis.wso2.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wso2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WSO2, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: WSO2
provider_slug: wso2
slug: wso2-domain-security
source_filename: wso2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wso2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apim.docs.wso2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 04:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apis.wso2.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wso2.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wso2/refs/heads/main/security/wso2-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- API Management
- Gateways
- Open Source
- API Lifecycle
- GraphQL
- SOAP
- REST
---
