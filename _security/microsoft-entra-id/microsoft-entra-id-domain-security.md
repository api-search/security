---
api_specs:
- filename: microsoft-entra-id-applications-api-openapi.yml
  format: yaml
  label: Microsoft Entra ID Applications API
  slug: microsoft-entra-id-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-applications-api-openapi.yml
- filename: microsoft-entra-id-directoryroles-api-openapi.yml
  format: yaml
  label: Microsoft Entra ID DirectoryRoles API
  slug: microsoft-entra-id-directoryroles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-directoryroles-api-openapi.yml
- filename: microsoft-entra-id-groups-api-openapi.yml
  format: yaml
  label: Microsoft Entra ID Groups API
  slug: microsoft-entra-id-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-groups-api-openapi.yml
- filename: microsoft-entra-id-serviceprincipals-api-openapi.yml
  format: yaml
  label: Microsoft Entra ID ServicePrincipals API
  slug: microsoft-entra-id-serviceprincipals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-serviceprincipals-api-openapi.yml
- filename: microsoft-entra-id-users-api-openapi.yml
  format: yaml
  label: Microsoft Entra ID Users API
  slug: microsoft-entra-id-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/openapi/microsoft-entra-id-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  2 03:53:00 2026 GMT
  host: graph.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Entra Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Entra ID, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Entra ID
provider_slug: microsoft-entra-id
slug: microsoft-entra-id-domain-security
source_filename: microsoft-entra-id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: graph.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 03:53:00 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-entra-id/refs/heads/main/security/microsoft-entra-id-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Authentication
- Identity Provider
---
