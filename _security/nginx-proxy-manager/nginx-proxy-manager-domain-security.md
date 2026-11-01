---
api_specs:
- filename: nginx-proxy-manager-audit-log-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Audit Log API
  slug: nginx-proxy-manager-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-audit-log-api-openapi.yml
- filename: nginx-proxy-manager-logs-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Logs API
  slug: nginx-proxy-manager-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-logs-api-openapi.yml
- filename: nginx-proxy-manager-nginx-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Nginx API
  slug: nginx-proxy-manager-nginx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-nginx-api-openapi.yml
- filename: nginx-proxy-manager-nginx-proxy-manager-api-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Nginx Proxy Manager API
  slug: nginx-proxy-manager-nginx-proxy-manager-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-nginx-proxy-manager-api-api-openapi.yml
- filename: nginx-proxy-manager-reports-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Reports API
  slug: nginx-proxy-manager-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-reports-api-openapi.yml
- filename: nginx-proxy-manager-schema-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Schema API
  slug: nginx-proxy-manager-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-schema-api-openapi.yml
- filename: nginx-proxy-manager-settings-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Settings API
  slug: nginx-proxy-manager-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-settings-api-openapi.yml
- filename: nginx-proxy-manager-tokens-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Tokens API
  slug: nginx-proxy-manager-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-tokens-api-openapi.yml
- filename: nginx-proxy-manager-users-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Users API
  slug: nginx-proxy-manager-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-users-api-openapi.yml
- filename: nginx-proxy-manager-version-api-openapi.yml
  format: yaml
  label: Nginx Proxy Manager Version API
  slug: nginx-proxy-manager-version-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nginx-proxy-manager/openapi/nginx-proxy-manager-version-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: nginxproxymanager.com
  spf: true
hosts:
- cert_expires: Dec 15 20:35:11 2026 GMT
  host: nginxproxymanager.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Nginx Proxy Manager Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Nginx Proxy Manager, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Nginx Proxy Manager
provider_slug: nginx-proxy-manager
slug: nginx-proxy-manager-domain-security
source_filename: nginx-proxy-manager-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: nginxproxymanager.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 15 20:35:11 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: nginxproxymanager.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/nginx-proxy-manager/security/nginx-proxy-manager-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- OpenSource
- Docker
- Nginx
- Proxy
- SSL
---
