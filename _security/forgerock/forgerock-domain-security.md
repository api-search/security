---
api_specs:
- filename: forgerock-identity-cloud-openapi.yml
  format: yaml
  label: ForgeRock Identity Cloud REST API
  slug: forgerock-identity-cloud-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-cloud-openapi.yml
- filename: forgerock-access-management-openapi.yml
  format: yaml
  label: ForgeRock Access Management API
  slug: forgerock-access-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-access-management-openapi.yml
- filename: forgerock-identity-management-openapi.yml
  format: yaml
  label: ForgeRock Identity Management API
  slug: forgerock-identity-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-management-openapi.yml
- filename: forgerock-identity-gateway-openapi.yml
  format: yaml
  label: ForgeRock Identity Gateway API
  slug: forgerock-identity-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-gateway-openapi.yml
- filename: forgerock-directory-services-openapi.yml
  format: yaml
  label: ForgeRock Directory Services API
  slug: forgerock-directory-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-directory-services-openapi.yml
- filename: forgerock-identity-governance-openapi.yml
  format: yaml
  label: ForgeRock Identity Governance API
  slug: forgerock-identity-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-identity-governance-openapi.yml
- filename: forgerock-autonomous-identity-openapi.yml
  format: yaml
  label: ForgeRock Autonomous Identity API
  slug: forgerock-autonomous-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/openapi/forgerock-autonomous-identity-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:sysadmin@forgerock.com"
  - 0 issue "amazonaws.com"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: forgerock.com
  spf: true
hosts:
- cert_expires: Aug 22 17:27:17 2026 GMT
  host: backstage.forgerock.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: www.forgerock.com
  hsts: true
  hsts_max_age: 31557600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Forgerock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ForgeRock, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ForgeRock
provider_slug: forgerock
slug: forgerock-domain-security
source_filename: forgerock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: backstage.forgerock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 17:27:17 2026 GMT\n  hsts: false\n- host: www.forgerock.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31557600\ndomains:\n- domain: forgerock.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:sysadmin@forgerock.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forgerock/refs/heads/main/security/forgerock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Access Management
- Authentication
- Authorization
- Identity Governance
- Identity Management
- OAuth
- OpenID Connect
---
