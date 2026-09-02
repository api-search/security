---
api_specs:
- filename: powershell-metadata-api-openapi.yml
  format: yaml
  label: PowerShell Metadata API
  slug: powershell-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/openapi/powershell-metadata-api-openapi.yml
- filename: powershell-packages-api-openapi.yml
  format: yaml
  label: PowerShell Packages API
  slug: powershell-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/openapi/powershell-packages-api-openapi.yml
- filename: powershell-search-api-openapi.yml
  format: yaml
  label: PowerShell Search API
  slug: powershell-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/openapi/powershell-search-api-openapi.yml
- filename: powershell-updates-api-openapi.yml
  format: yaml
  label: PowerShell Updates API
  slug: powershell-updates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/openapi/powershell-updates-api-openapi.yml
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
  - 0 iodef "mailto:caarecordaware@microsoft.com"
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: powershellgallery.com
  spf: false
hosts:
- cert_expires: Dec 20 09:04:17 2026 GMT
  host: microsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: www.powershellgallery.com
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
name: Powershell Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PowerShell, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: PowerShell
provider_slug: powershell
slug: powershell-domain-security
source_filename: powershell-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 09:04:17 2026 GMT\n  hsts: false\n- host: www.powershellgallery.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 06:59:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: powershellgallery.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caarecordaware@microsoft.com\"\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powershell/refs/heads/main/security/powershell-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automation
- Command Line
- Cross-Platform
- Scripting
- Shell
- Windows
- DevOps
---
