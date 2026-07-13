---
api_specs:
- filename: overview
  format: yaml
  label: ASP.NET Core Web API
  slug: aspnet-core-web-api
  spec_type: OpenAPI
  url: https://learn.microsoft.com/en-us/aspnet/core/fundamentals/openapi/overview
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
- cert_expires: Nov 23 17:38:27 2026 GMT
  host: dotnet.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Microsoft Dotnet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Microsoft .NET, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Microsoft .NET
provider_slug: microsoft-dotnet
slug: microsoft-dotnet-domain-security
source_filename: microsoft-dotnet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dotnet.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 23 17:38:27 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/microsoft-dotnet/refs/heads/main/security/microsoft-dotnet-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- .NET
- ASP.NET Core
- Azure SDK
- Cross-Platform
- Framework
- Runtime
- Web API
---
