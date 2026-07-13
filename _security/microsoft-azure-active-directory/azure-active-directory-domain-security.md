---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Microsoft Graph API
  slug: microsoft-graph-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/microsoftgraph/msgraph-metadata/master/openapi/v1.0/openapi.yaml
- filename: microsoft-graph-identity-api.yml
  format: yaml
  label: Microsoft Graph Identity and Access API
  slug: microsoft-graph-identity-and-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/openapi/microsoft-graph-identity-api.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan  5 19:53:18 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 15 18:01:46 2026 GMT
  host: entra.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 10 06:59:10 2026 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Azure Active Directory Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Azure Active Directory, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Azure Active Directory
provider_slug: microsoft-azure-active-directory
slug: azure-active-directory-domain-security
source_filename: azure-active-directory-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  5 19:53:18 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: entra.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 18:01:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-azure-active-directory/refs/heads/main/security/azure-active-directory-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- Microsoft
- Microsoft Entra
- OAuth
- OpenID Connect
- SAML
- SCIM
- Single Sign-On
- Zero Trust
---
