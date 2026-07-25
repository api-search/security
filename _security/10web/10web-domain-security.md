---
api_specs:
- filename: 10web-account-api-openapi.yml
  format: yaml
  label: 10Web Account API
  slug: 10web-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-account-api-openapi.yml
- filename: 10web-backup-api-openapi.yml
  format: yaml
  label: 10Web Backup API
  slug: 10web-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-backup-api-openapi.yml
- filename: 10web-builder-api-openapi.yml
  format: yaml
  label: 10Web Builder API
  slug: 10web-builder-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-builder-api-openapi.yml
- filename: 10web-cache-api-openapi.yml
  format: yaml
  label: 10Web Cache API
  slug: 10web-cache-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-cache-api-openapi.yml
- filename: 10web-certificate-api-openapi.yml
  format: yaml
  label: 10Web Certificate API
  slug: 10web-certificate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-certificate-api-openapi.yml
- filename: 10web-domain-api-openapi.yml
  format: yaml
  label: 10Web Domain API
  slug: 10web-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-domain-api-openapi.yml
- filename: 10web-php-management-api-openapi.yml
  format: yaml
  label: 10Web PHP Management API
  slug: 10web-php-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-php-management-api-openapi.yml
- filename: 10web-section-based-ai-api-openapi.yml
  format: yaml
  label: 10Web Section Based AI API
  slug: 10web-section-based-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-section-based-ai-api-openapi.yml
- filename: 10web-subdomain-api-openapi.yml
  format: yaml
  label: 10Web Subdomain API
  slug: 10web-subdomain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-subdomain-api-openapi.yml
- filename: 10web-vibe-coding-api-openapi.yml
  format: yaml
  label: 10Web Vibe Coding API
  slug: 10web-vibe-coding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-vibe-coding-api-openapi.yml
- filename: 10web-website-api-openapi.yml
  format: yaml
  label: 10Web Website API
  slug: 10web-website-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-website-api-openapi.yml
- filename: 10web-wp-autologin-api-openapi.yml
  format: yaml
  label: 10Web WP Autologin API
  slug: 10web-wp-autologin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-wp-autologin-api-openapi.yml
- filename: 10web-zone-api-openapi.yml
  format: yaml
  label: 10Web Zone API
  slug: 10web-zone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/openapi/10web-zone-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: 10web.io
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: 10web.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 09:58:22 2026 GMT
  host: api.10web.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 10Web Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 10Web, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: 10Web
provider_slug: 10web
slug: 10web-domain-security
source_filename: 10web-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: 10web.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.10web.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 09:58:22 2026 GMT\n  hsts: null\ndomains:\n- domain: 10web.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/10web/refs/heads/main/security/10web-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Website Builder
- WordPress
- Hosting
- Website Generation
- No-Code
---
