---
api_specs:
- filename: juvenescence-posts-api-openapi.yml
  format: yaml
  label: Juvenescence Posts API
  slug: juvenescence-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-posts-api-openapi.yml
- filename: juvenescence-pages-api-openapi.yml
  format: yaml
  label: Juvenescence Pages API
  slug: juvenescence-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-pages-api-openapi.yml
- filename: juvenescence-media-api-openapi.yml
  format: yaml
  label: Juvenescence Media API
  slug: juvenescence-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-media-api-openapi.yml
- filename: juvenescence-categories-api-openapi.yml
  format: yaml
  label: Juvenescence Categories API
  slug: juvenescence-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-categories-api-openapi.yml
- filename: juvenescence-tags-api-openapi.yml
  format: yaml
  label: Juvenescence Tags API
  slug: juvenescence-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-tags-api-openapi.yml
- filename: juvenescence-comments-api-openapi.yml
  format: yaml
  label: Juvenescence Comments API
  slug: juvenescence-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-comments-api-openapi.yml
- filename: juvenescence-search-api-openapi.yml
  format: yaml
  label: Juvenescence Search API
  slug: juvenescence-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-search-api-openapi.yml
- filename: juvenescence-portfolio-api-openapi.yml
  format: yaml
  label: Juvenescence Portfolio API
  slug: juvenescence-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-portfolio-api-openapi.yml
- filename: juvenescence-discovery-api-openapi.yml
  format: yaml
  label: Juvenescence Discovery API
  slug: juvenescence-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/openapi/juvenescence-discovery-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: juvlabs.com
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
- cert_expires: Oct 11 13:04:02 2026 GMT
  host: juvlabs.com
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
name: Juvenescence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Juvenescence, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Juvenescence
provider_slug: juvenescence
slug: juvenescence-domain-security
source_filename: juvenescence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: juvlabs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 13:04:02 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: juvlabs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/juvenescence/refs/heads/main/security/juvenescence-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Longevity
- Drug Discovery
- Life Sciences
- Clinical Trials
- Artificial Intelligence
- Aging
- content-api
---
