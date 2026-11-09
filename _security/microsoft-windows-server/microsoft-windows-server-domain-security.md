---
api_specs:
- filename: microsoft-windows-server-application-pools-api-openapi.yml
  format: yaml
  label: Microsoft Windows Server Application Pools API
  slug: microsoft-windows-server-application-pools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-windows-server/openapi/microsoft-windows-server-application-pools-api-openapi.yml
- filename: microsoft-windows-server-applications-api-openapi.yml
  format: yaml
  label: Microsoft Windows Server Applications API
  slug: microsoft-windows-server-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-windows-server/openapi/microsoft-windows-server-applications-api-openapi.yml
- filename: microsoft-windows-server-websites-api-openapi.yml
  format: yaml
  label: Microsoft Windows Server Websites API
  slug: microsoft-windows-server-websites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-windows-server/openapi/microsoft-windows-server-websites-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
hosts:
- cert_expires: Jan 17 19:55:21 2027 GMT
  host: www.microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  7 23:37:09 2027 GMT
  host: docs.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Microsoft Windows Server Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft Windows Server, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft Windows Server
provider_slug: microsoft-windows-server
slug: microsoft-windows-server-domain-security
source_filename: microsoft-windows-server-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 19:55:21 2027 GMT\n  hsts: false\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  7 23:37:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-windows-server/security/microsoft-windows-server-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data Center
- Enterprise
- Infrastructure
- Microsoft
- Operating System
- Server Management
- Windows Server
- Windows Server 2025
---
