---
api_specs:
- filename: skrime-account-api-openapi.yml
  format: yaml
  label: SKRIME Account API
  slug: skrime-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-account-api-openapi.yml
- filename: skrime-asn-api-openapi.yml
  format: yaml
  label: SKRIME Asn API
  slug: skrime-asn-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-asn-api-openapi.yml
- filename: skrime-dedicated-api-openapi.yml
  format: yaml
  label: SKRIME Dedicated API
  slug: skrime-dedicated-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-dedicated-api-openapi.yml
- filename: skrime-dns-api-openapi.yml
  format: yaml
  label: SKRIME Dns API
  slug: skrime-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-dns-api-openapi.yml
- filename: skrime-domain-api-openapi.yml
  format: yaml
  label: SKRIME Domain API
  slug: skrime-domain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-domain-api-openapi.yml
- filename: skrime-instance-api-openapi.yml
  format: yaml
  label: SKRIME Instance API
  slug: skrime-instance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-instance-api-openapi.yml
- filename: skrime-ipv4-api-openapi.yml
  format: yaml
  label: SKRIME Ipv4 API
  slug: skrime-ipv4-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-ipv4-api-openapi.yml
- filename: skrime-ipv6-api-openapi.yml
  format: yaml
  label: SKRIME Ipv6 API
  slug: skrime-ipv6-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-ipv6-api-openapi.yml
- filename: skrime-other-api-openapi.yml
  format: yaml
  label: SKRIME Other API
  slug: skrime-other-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-other-api-openapi.yml
- filename: skrime-product-api-openapi.yml
  format: yaml
  label: SKRIME Product API
  slug: skrime-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-product-api-openapi.yml
- filename: skrime-proxmox-backup-api-openapi.yml
  format: yaml
  label: SKRIME Proxmox Backup API
  slug: skrime-proxmox-backup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-proxmox-backup-api-openapi.yml
- filename: skrime-server-api-openapi.yml
  format: yaml
  label: SKRIME Server API
  slug: skrime-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-server-api-openapi.yml
- filename: skrime-ssl-api-openapi.yml
  format: yaml
  label: SKRIME Ssl API
  slug: skrime-ssl-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-ssl-api-openapi.yml
- filename: skrime-status-api-openapi.yml
  format: yaml
  label: SKRIME Status API
  slug: skrime-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-status-api-openapi.yml
- filename: skrime-statuspage-api-openapi.yml
  format: yaml
  label: SKRIME Statuspage API
  slug: skrime-statuspage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-statuspage-api-openapi.yml
- filename: skrime-support-api-openapi.yml
  format: yaml
  label: SKRIME Support API
  slug: skrime-support-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-support-api-openapi.yml
- filename: skrime-webspace-api-openapi.yml
  format: yaml
  label: SKRIME Webspace API
  slug: skrime-webspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/skrime/openapi/skrime-webspace-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: skrime.eu
  spf: true
hosts:
- cert_expires: Jan  1 05:24:56 2027 GMT
  host: skrime.eu
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: SKRIME Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SKRIME, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: SKRIME
provider_slug: skrime
slug: skrime-domain-security
source_filename: skrime-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: skrime.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  1 05:24:56 2027 GMT\n  hsts: null\ndomains:\n- domain: skrime.eu\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/skrime/security/skrime-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cloud
- Hosting
- Infrastructure
- EU
---
