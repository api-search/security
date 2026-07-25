---
api_specs:
- filename: nuget-catalog-api-openapi.yml
  format: yaml
  label: NuGet Catalog API
  slug: nuget-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-catalog-api-openapi.yml
- filename: nuget-search-api-openapi.yml
  format: yaml
  label: NuGet Search API
  slug: nuget-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-search-api-openapi.yml
- filename: nuget-package-content-api-openapi.yml
  format: yaml
  label: NuGet Package Content API
  slug: nuget-package-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-package-content-api-openapi.yml
- filename: nuget-autocomplete-api-openapi.yml
  format: yaml
  label: NuGet Autocomplete API
  slug: nuget-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-autocomplete-api-openapi.yml
- filename: nuget-package-publish-api-openapi.yml
  format: yaml
  label: NuGet Package Publish API
  slug: nuget-package-publish-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-package-publish-api-openapi.yml
- filename: nuget-registration-api-openapi.yml
  format: yaml
  label: NuGet Registration API
  slug: nuget-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-registration-api-openapi.yml
- filename: nuget-service-index-api-openapi.yml
  format: yaml
  label: NuGet Service Index API
  slug: nuget-service-index-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/openapi/nuget-service-index-api-openapi.yml
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
  domain: nuget.org
  spf: true
hosts:
- cert_expires: Dec 11 02:26:09 2026 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 13:23:07 2026 GMT
  host: www.nuget.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 13:23:07 2026 GMT
  host: api.nuget.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Nuget Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NuGet, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NuGet
provider_slug: nuget
slug: nuget-domain-security
source_filename: nuget-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 02:26:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.nuget.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 13:23:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.nuget.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 13:23:07 2026 GMT\n  hsts: null\ndomains:\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: nuget.org\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuget/refs/heads/main/security/nuget-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Package Management
- .NET
- Packages
- Dependencies
- Software Distribution
- Registry
---
