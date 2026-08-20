---
api_specs:
- filename: wiktionary-definition-api-openapi.yml
  format: yaml
  label: Wiktionary Definition API
  slug: wiktionary-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-definition-api-openapi.yml
- filename: wiktionary-expandtemplates-api-openapi.yml
  format: yaml
  label: Wiktionary ExpandTemplates API
  slug: wiktionary-expandtemplates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-expandtemplates-api-openapi.yml
- filename: wiktionary-file-api-openapi.yml
  format: yaml
  label: Wiktionary File API
  slug: wiktionary-file-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-file-api-openapi.yml
- filename: wiktionary-history-api-openapi.yml
  format: yaml
  label: Wiktionary History API
  slug: wiktionary-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-history-api-openapi.yml
- filename: wiktionary-opensearch-api-openapi.yml
  format: yaml
  label: Wiktionary OpenSearch API
  slug: wiktionary-opensearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-opensearch-api-openapi.yml
- filename: wiktionary-page-api-openapi.yml
  format: yaml
  label: Wiktionary Page API
  slug: wiktionary-page-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-page-api-openapi.yml
- filename: wiktionary-page-content-api-openapi.yml
  format: yaml
  label: Wiktionary Page Content API
  slug: wiktionary-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-page-content-api-openapi.yml
- filename: wiktionary-parse-api-openapi.yml
  format: yaml
  label: Wiktionary Parse API
  slug: wiktionary-parse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-parse-api-openapi.yml
- filename: wiktionary-query-api-openapi.yml
  format: yaml
  label: Wiktionary Query API
  slug: wiktionary-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-query-api-openapi.yml
- filename: wiktionary-search-api-openapi.yml
  format: yaml
  label: Wiktionary Search API
  slug: wiktionary-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-search-api-openapi.yml
- filename: wiktionary-transform-api-openapi.yml
  format: yaml
  label: Wiktionary Transform API
  slug: wiktionary-transform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/openapi/wiktionary-transform-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wiktionary.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wiktionary.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wiktionary Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wiktionary, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wiktionary
provider_slug: wiktionary
slug: wiktionary-domain-security
source_filename: wiktionary-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wiktionary.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wiktionary.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wiktionary/refs/heads/main/security/wiktionary-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Dictionaries
- Open-Source
- Wikimedia
- MediaWiki
- Linguistics
- Open Data
- Public APIs
---
