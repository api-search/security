---
api_specs:
- filename: abcuro-careers-api-openapi.yml
  format: yaml
  label: Abcuro Careers API
  slug: abcuro-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-careers-api-openapi.yml
- filename: abcuro-comments-api-openapi.yml
  format: yaml
  label: Abcuro Comments API
  slug: abcuro-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-comments-api-openapi.yml
- filename: abcuro-discovery-api-openapi.yml
  format: yaml
  label: Abcuro Discovery API
  slug: abcuro-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-discovery-api-openapi.yml
- filename: abcuro-investors-api-openapi.yml
  format: yaml
  label: Abcuro Investors API
  slug: abcuro-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-investors-api-openapi.yml
- filename: abcuro-media-api-openapi.yml
  format: yaml
  label: Abcuro Media API
  slug: abcuro-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-media-api-openapi.yml
- filename: abcuro-pages-api-openapi.yml
  format: yaml
  label: Abcuro Pages API
  slug: abcuro-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-pages-api-openapi.yml
- filename: abcuro-people-api-openapi.yml
  format: yaml
  label: Abcuro People API
  slug: abcuro-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-people-api-openapi.yml
- filename: abcuro-press-releases-api-openapi.yml
  format: yaml
  label: Abcuro Press Releases API
  slug: abcuro-press-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-press-releases-api-openapi.yml
- filename: abcuro-publications-api-openapi.yml
  format: yaml
  label: Abcuro Publications API
  slug: abcuro-publications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-publications-api-openapi.yml
- filename: abcuro-search-api-openapi.yml
  format: yaml
  label: Abcuro Search API
  slug: abcuro-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-search-api-openapi.yml
- filename: abcuro-taxonomy-api-openapi.yml
  format: yaml
  label: Abcuro Taxonomy API
  slug: abcuro-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-taxonomy-api-openapi.yml
- filename: abcuro-users-api-openapi.yml
  format: yaml
  label: Abcuro Users API
  slug: abcuro-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/openapi/abcuro-users-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: abcuro.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143"
  - 0 iodef "mailto:caa@wordpress.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wordpress.org
  spf: true
hosts:
- cert_expires: Sep 25 01:57:06 2026 GMT
  host: abcuro.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 23 19:43:55 2026 GMT
  host: developer.wordpress.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Abcuro Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abcuro, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Abcuro
provider_slug: abcuro
slug: abcuro-domain-security
source_filename: abcuro-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abcuro.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 25 01:57:06 2026 GMT\n  hsts: false\n- host: developer.wordpress.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:43:55 2026 GMT\n  hsts: false\ndomains:\n- domain: abcuro.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: wordpress.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/53691143\"\n  - 0 iodef \"mailto:caa@wordpress.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abcuro/refs/heads/main/security/abcuro-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Biotechnology
- Pharmaceuticals
- Immunology
- Autoimmune Disease
- Oncology
- Clinical Trials
- Life Sciences
- Drug Development
- Healthcare
- content-api
- WordPress
---
