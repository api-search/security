---
api_specs:
- filename: wpengine-account-api-openapi.yml
  format: yaml
  label: WP Engine Account API
  slug: wpengine-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-account-api-openapi.yml
- filename: wpengine-account-user-api-openapi.yml
  format: yaml
  label: WP Engine Account User API
  slug: wpengine-account-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-account-user-api-openapi.yml
- filename: wpengine-archive-api-openapi.yml
  format: yaml
  label: WP Engine Archive API
  slug: wpengine-archive-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-archive-api-openapi.yml
- filename: wpengine-backup-api-openapi.yml
  format: yaml
  label: WP Engine Backup API
  slug: wpengine-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-backup-api-openapi.yml
- filename: wpengine-cache-api-openapi.yml
  format: yaml
  label: WP Engine Cache API
  slug: wpengine-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-cache-api-openapi.yml
- filename: wpengine-certificates-api-openapi.yml
  format: yaml
  label: WP Engine Certificates API
  slug: wpengine-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-certificates-api-openapi.yml
- filename: wpengine-domain-api-openapi.yml
  format: yaml
  label: WP Engine Domain API
  slug: wpengine-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-domain-api-openapi.yml
- filename: wpengine-install-api-openapi.yml
  format: yaml
  label: WP Engine Install API
  slug: wpengine-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-install-api-openapi.yml
- filename: wpengine-offload-settings-api-openapi.yml
  format: yaml
  label: WP Engine Offload Settings API
  slug: wpengine-offload-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-offload-settings-api-openapi.yml
- filename: wpengine-site-api-openapi.yml
  format: yaml
  label: WP Engine Site API
  slug: wpengine-site-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-site-api-openapi.yml
- filename: wpengine-site-reports-api-openapi.yml
  format: yaml
  label: WP Engine Site Reports API
  slug: wpengine-site-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-site-reports-api-openapi.yml
- filename: wpengine-site-transfer-api-openapi.yml
  format: yaml
  label: WP Engine Site Transfer API
  slug: wpengine-site-transfer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-site-transfer-api-openapi.yml
- filename: wpengine-ssh-key-api-openapi.yml
  format: yaml
  label: WP Engine SSH Key API
  slug: wpengine-ssh-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-ssh-key-api-openapi.yml
- filename: wpengine-status-api-openapi.yml
  format: yaml
  label: WP Engine Status API
  slug: wpengine-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-status-api-openapi.yml
- filename: wpengine-swagger-api-openapi.yml
  format: yaml
  label: WP Engine Swagger API
  slug: wpengine-swagger-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-swagger-api-openapi.yml
- filename: wpengine-usage-api-openapi.yml
  format: yaml
  label: WP Engine Usage API
  slug: wpengine-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-usage-api-openapi.yml
- filename: wpengine-user-api-openapi.yml
  format: yaml
  label: WP Engine User API
  slug: wpengine-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/openapi/wpengine-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wpengine.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wpengineapi.com
  spf: false
hosts:
- cert_expires: Oct  7 02:08:09 2026 GMT
  host: wpengine.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 06:04:18 2026 GMT
  host: developers.wpengine.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: api.wpengineapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wpengine Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WP Engine, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WP Engine
provider_slug: wpengine
slug: wpengine-domain-security
source_filename: wpengine-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wpengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:08:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.wpengine.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 06:04:18 2026 GMT\n  hsts: false\n- host: api.wpengineapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wpengine.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wpengineapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wpengine/refs/heads/main/security/wpengine-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- WordPress
- Managed Hosting
- WordPress Hosting
- Site Management
- Digital Experience Platform
---
