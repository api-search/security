---
api_specs:
- filename: wikivoyage-authentication-api-openapi.yml
  format: yaml
  label: Wikivoyage Authentication API
  slug: wikivoyage-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-authentication-api-openapi.yml
- filename: wikivoyage-edit-api-openapi.yml
  format: yaml
  label: Wikivoyage Edit API
  slug: wikivoyage-edit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-edit-api-openapi.yml
- filename: wikivoyage-files-api-openapi.yml
  format: yaml
  label: Wikivoyage Files API
  slug: wikivoyage-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-files-api-openapi.yml
- filename: wikivoyage-history-api-openapi.yml
  format: yaml
  label: Wikivoyage History API
  slug: wikivoyage-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-history-api-openapi.yml
- filename: wikivoyage-links-api-openapi.yml
  format: yaml
  label: Wikivoyage Links API
  slug: wikivoyage-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-links-api-openapi.yml
- filename: wikivoyage-meta-api-openapi.yml
  format: yaml
  label: Wikivoyage Meta API
  slug: wikivoyage-meta-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-meta-api-openapi.yml
- filename: wikivoyage-pages-api-openapi.yml
  format: yaml
  label: Wikivoyage Pages API
  slug: wikivoyage-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-pages-api-openapi.yml
- filename: wikivoyage-parse-api-openapi.yml
  format: yaml
  label: Wikivoyage Parse API
  slug: wikivoyage-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-parse-api-openapi.yml
- filename: wikivoyage-patrol-api-openapi.yml
  format: yaml
  label: Wikivoyage Patrol API
  slug: wikivoyage-patrol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-patrol-api-openapi.yml
- filename: wikivoyage-query-api-openapi.yml
  format: yaml
  label: Wikivoyage Query API
  slug: wikivoyage-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-query-api-openapi.yml
- filename: wikivoyage-revisions-api-openapi.yml
  format: yaml
  label: Wikivoyage Revisions API
  slug: wikivoyage-revisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-revisions-api-openapi.yml
- filename: wikivoyage-search-api-openapi.yml
  format: yaml
  label: Wikivoyage Search API
  slug: wikivoyage-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-search-api-openapi.yml
- filename: wikivoyage-transforms-api-openapi.yml
  format: yaml
  label: Wikivoyage Transforms API
  slug: wikivoyage-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-transforms-api-openapi.yml
- filename: wikivoyage-upload-api-openapi.yml
  format: yaml
  label: Wikivoyage Upload API
  slug: wikivoyage-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-upload-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikivoyage.org
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mediawiki.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: www.wikivoyage.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikivoyage.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: www.mediawiki.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wikivoyage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikivoyage, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wikivoyage
provider_slug: wikivoyage
slug: wikivoyage-domain-security
source_filename: wikivoyage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wikivoyage.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: en.wikivoyage.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: www.mediawiki.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wikivoyage.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mediawiki.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/security/wikivoyage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Open Data
- Public APIs
- Open Knowledge
- Travel Guide
- Tourism
- MediaWiki
- Non-Profit
---
