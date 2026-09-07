---
api_specs:
- filename: azure-ad-graph-applications-openapi.yml
  format: yaml
  label: Azure Active Directory Applications API
  slug: azure-ad-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-applications-openapi.yml
- filename: azure-ad-graph-identity-directorymanagement-openapi.yml
  format: yaml
  label: Azure Active Directory Directory API
  slug: azure-ad-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-directorymanagement-openapi.yml
- filename: azure-ad-graph-groups-openapi.yml
  format: yaml
  label: Azure Active Directory Groups API
  slug: azure-ad-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-groups-openapi.yml
- filename: azure-ad-me-api-openapi.yml
  format: yaml
  label: Azure Active Directory Me API
  slug: azure-ad-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/azure-ad-me-api-openapi.yml
- filename: azure-ad-graph-users-openapi.yml
  format: yaml
  label: Azure Active Directory Users API
  slug: azure-ad-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-users-openapi.yml
- filename: azure-ad-graph-identity-signins-openapi.yml
  format: yaml
  label: Microsoft Entra ID Sign-Ins and Policies API
  slug: azure-ad-signins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-signins-openapi.yml
- filename: azure-ad-graph-identity-governance-openapi.yml
  format: yaml
  label: Microsoft Entra ID Governance API
  slug: azure-ad-governance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-identity-governance-openapi.yml
- filename: azure-ad-graph-directoryobjects-openapi.yml
  format: yaml
  label: Microsoft Entra ID Directory Objects API
  slug: azure-ad-directory-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-directoryobjects-openapi.yml
- filename: azure-ad-graph-changenotifications-openapi.yml
  format: yaml
  label: Microsoft Entra ID Change Notifications API
  slug: azure-ad-change-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/openapi/_original/azure-ad-graph-changenotifications-openapi.yml
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
- cert_expires: Feb 25 12:39:07 2027 GMT
  host: portal.azure.com
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
- cert_expires: Nov 22 03:32:13 2026 GMT
  host: login.microsoftonline.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure Ad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Entra ID (formerly Azure AD), probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Microsoft Entra ID (formerly Azure AD)
provider_slug: azure-ad
slug: azure-ad-domain-security
source_filename: azure-ad-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 12:39:07 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: login.microsoftonline.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 03:32:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azure-ad/refs/heads/main/security/azure-ad-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Authentication
- Authorization
- Identity
- OpenID Connect
- Single Sign-On
---
