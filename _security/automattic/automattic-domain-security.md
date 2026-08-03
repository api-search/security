---
api_specs:
- filename: automattic-wordpress-com-rest-v1-1-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.1
  slug: wordpresscom-rest-api-v11
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-1-openapi.yml
- filename: automattic-wordpress-com-rest-v1-2-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.2
  slug: wordpresscom-rest-api-v12
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-2-openapi.yml
- filename: automattic-wordpress-com-rest-v1-3-openapi.yml
  format: yaml
  label: WordPress.com REST API v1.3
  slug: wordpresscom-rest-api-v13
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-rest-v1-3-openapi.yml
- filename: automattic-wordpress-com-wp-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wp/v2 namespace
  slug: wordpresscom-rest-api-wpv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wp-v2-openapi.yml
- filename: automattic-wordpress-com-wpcom-v2-openapi.yml
  format: yaml
  label: WordPress.com REST API - wpcom/v2 namespace
  slug: wordpresscom-rest-api-wpcomv2-namespace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-wordpress-com-wpcom-v2-openapi.yml
- filename: automattic-akismet-openapi.yml
  format: yaml
  label: Akismet API
  slug: akismet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-akismet-openapi.yml
- filename: automattic-jetpack-ai-plugin-openapi.yaml
  format: yaml
  label: Jetpack AI-Plugin API
  slug: jetpack-ai-plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/openapi/automattic-jetpack-ai-plugin-openapi.yaml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: automattic.com
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489"
  - 0 iodef "mailto:caa@automattic.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.com
  spf: true
hosts:
- cert_expires: Sep  9 19:43:59 2026 GMT
  host: automattic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:45:22 2026 GMT
  host: developer.wordpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 19:45:22 2026 GMT
  host: public-api.wordpress.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Automattic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Automattic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Automattic
provider_slug: automattic
slug: automattic-domain-security
source_filename: automattic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: automattic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 19:43:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.wordpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:45:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: public-api.wordpress.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 19:45:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: automattic.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wordpress.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489\"\n  - 0 iodef \"mailto:caa@automattic.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/36334489\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automattic/refs/heads/main/security/automattic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Content Management
- Publishing
- Blogging
- Website Hosting
- Web Publishing
- Content
- Comments
- Spam Filtering
- Media
- Analytics
- Domains
- E-Commerce
- Open Source
- Developer Tools
- Model Context Protocol
---
