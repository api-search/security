---
api_specs:
- filename: clusters-authentication-api-openapi.yml
  format: yaml
  label: Clusters Authentication API
  slug: clusters-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-authentication-api-openapi.yml
- filename: clusters-clusters-api-openapi.yml
  format: yaml
  label: Clusters Clusters API
  slug: clusters-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-clusters-api-openapi.yml
- filename: clusters-communities-api-openapi.yml
  format: yaml
  label: Clusters Communities API
  slug: clusters-communities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-communities-api-openapi.yml
- filename: clusters-events-api-openapi.yml
  format: yaml
  label: Clusters Events API
  slug: clusters-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-events-api-openapi.yml
- filename: clusters-names-api-openapi.yml
  format: yaml
  label: Clusters Names API
  slug: clusters-names-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-names-api-openapi.yml
- filename: clusters-registration-api-openapi.yml
  format: yaml
  label: Clusters Registration API
  slug: clusters-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/openapi/clusters-registration-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: clusters.xyz
  spf: false
hosts:
- cert_expires: Oct 16 18:34:22 2026 GMT
  host: clusters.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 04:39:19 2026 GMT
  host: docs.clusters.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 20:50:20 2026 GMT
  host: api.clusters.xyz
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Clusters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clusters, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Clusters
provider_slug: clusters
slug: clusters-domain-security
source_filename: clusters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clusters.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 18:34:22 2026 GMT\n  hsts: false\n- host: docs.clusters.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 04:39:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.clusters.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:50:20 2026 GMT\n  hsts: false\ndomains:\n- domain: clusters.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clusters/refs/heads/main/security/clusters-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Infrastructure
- Identity
- Naming
- Blockchain
- Web3
- Wallets
- Multichain
- Resolver
---
