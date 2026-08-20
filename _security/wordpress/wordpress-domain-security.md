---
api_specs:
- filename: wordpress-block-types-api-openapi.yml
  format: yaml
  label: WordPress Block Types API
  slug: wordpress-block-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-block-types-api-openapi.yml
- filename: wordpress-blocks-api-openapi.yml
  format: yaml
  label: WordPress Blocks API
  slug: wordpress-blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-blocks-api-openapi.yml
- filename: wordpress-categories-api-openapi.yml
  format: yaml
  label: WordPress Categories API
  slug: wordpress-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-categories-api-openapi.yml
- filename: wordpress-comments-api-openapi.yml
  format: yaml
  label: WordPress Comments API
  slug: wordpress-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-comments-api-openapi.yml
- filename: wordpress-media-api-openapi.yml
  format: yaml
  label: WordPress Media API
  slug: wordpress-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-media-api-openapi.yml
- filename: wordpress-pages-api-openapi.yml
  format: yaml
  label: WordPress Pages API
  slug: wordpress-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-pages-api-openapi.yml
- filename: wordpress-plugins-api-openapi.yml
  format: yaml
  label: WordPress Plugins API
  slug: wordpress-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-plugins-api-openapi.yml
- filename: wordpress-post-types-api-openapi.yml
  format: yaml
  label: WordPress Post Types API
  slug: wordpress-post-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-post-types-api-openapi.yml
- filename: wordpress-posts-api-openapi.yml
  format: yaml
  label: WordPress Posts API
  slug: wordpress-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-posts-api-openapi.yml
- filename: wordpress-search-api-openapi.yml
  format: yaml
  label: WordPress Search API
  slug: wordpress-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-search-api-openapi.yml
- filename: wordpress-settings-api-openapi.yml
  format: yaml
  label: WordPress Settings API
  slug: wordpress-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-settings-api-openapi.yml
- filename: wordpress-tags-api-openapi.yml
  format: yaml
  label: WordPress Tags API
  slug: wordpress-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-tags-api-openapi.yml
- filename: wordpress-themes-api-openapi.yml
  format: yaml
  label: WordPress Themes API
  slug: wordpress-themes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-themes-api-openapi.yml
- filename: wordpress-users-api-openapi.yml
  format: yaml
  label: WordPress Users API
  slug: wordpress-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/openapi/wordpress-users-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: wp-cli.org
  spf: false
hosts:
- cert_expires: Aug 24 19:43:58 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 19:44:09 2026 GMT
  host: wp-cli.org
  hsts: true
  hsts_max_age: 3600
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wordpress Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WordPress, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: WordPress
provider_slug: wordpress
slug: wordpress-domain-security
source_filename: wordpress-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 19:43:58 2026 GMT\n  hsts: false\n- host: wp-cli.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 19:44:09 2026 GMT\n  hsts: true\n  hsts_max_age: 3600\ndomains:\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wp-cli.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordpress/refs/heads/main/security/wordpress-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Management
- Open-Source
- WordPress
---
