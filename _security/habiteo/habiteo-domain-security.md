---
api_specs:
- filename: habiteo-posts-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Posts API
  slug: posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-posts-api-openapi.yml
- filename: habiteo-pages-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Pages API
  slug: pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-pages-api-openapi.yml
- filename: habiteo-media-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Media API
  slug: media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-media-api-openapi.yml
- filename: habiteo-portfolio-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Portfolio API
  slug: portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-portfolio-api-openapi.yml
- filename: habiteo-blocks-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Blocks API
  slug: blocks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-blocks-api-openapi.yml
- filename: habiteo-taxonomy-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Taxonomy API
  slug: taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-taxonomy-api-openapi.yml
- filename: habiteo-discovery-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Discovery API
  slug: discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-discovery-api-openapi.yml
- filename: habiteo-users-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Users API
  slug: users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-users-api-openapi.yml
- filename: habiteo-comments-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Comments API
  slug: comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-comments-api-openapi.yml
- filename: habiteo-settings-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Settings API
  slug: settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-settings-api-openapi.yml
- filename: habiteo-contact-forms-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Contact Forms API
  slug: contact-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-contact-forms-api-openapi.yml
- filename: habiteo-oembed-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — oEmbed API
  slug: oembed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-oembed-api-openapi.yml
- filename: habiteo-site-tools-api-openapi.yml
  format: yaml
  label: Habiteo Site Content API — Site Tools API
  slug: site-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/openapi/habiteo-site-tools-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: habiteo.com
  spf: true
- caa:
  - 0 iodef "mailto:caa@wordpress.org"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Dec 16 23:59:59 2026 GMT
  host: www.habiteo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Habiteo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Habiteo, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Habiteo
provider_slug: habiteo
slug: habiteo-domain-security
source_filename: habiteo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.habiteo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 23:59:59 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: habiteo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habiteo/refs/heads/main/security/habiteo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Real Estate
- PropTech
- 3D Visualization
- Property Marketing
- Configurator
- CRM
- France
- Content
- WordPress
---
