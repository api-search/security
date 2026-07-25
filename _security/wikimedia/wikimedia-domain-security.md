---
api_specs:
- filename: wikimedia-articles-api-openapi.yml
  format: yaml
  label: Wikimedia articles API
  slug: wikimedia-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-articles-api-openapi.yml
- filename: wikimedia-batches-api-openapi.yml
  format: yaml
  label: Wikimedia batches API
  slug: wikimedia-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-batches-api-openapi.yml
- filename: wikimedia-citation-api-openapi.yml
  format: yaml
  label: Wikimedia Citation API
  slug: wikimedia-citation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-citation-api-openapi.yml
- filename: wikimedia-codes-api-openapi.yml
  format: yaml
  label: Wikimedia codes API
  slug: wikimedia-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-codes-api-openapi.yml
- filename: wikimedia-languages-api-openapi.yml
  format: yaml
  label: Wikimedia languages API
  slug: wikimedia-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-languages-api-openapi.yml
- filename: wikimedia-math-api-openapi.yml
  format: yaml
  label: Wikimedia Math API
  slug: wikimedia-math-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-math-api-openapi.yml
- filename: wikimedia-mobile-api-openapi.yml
  format: yaml
  label: Wikimedia Mobile API
  slug: wikimedia-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-mobile-api-openapi.yml
- filename: wikimedia-namespaces-api-openapi.yml
  format: yaml
  label: Wikimedia namespaces API
  slug: wikimedia-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-namespaces-api-openapi.yml
- filename: wikimedia-offline-api-openapi.yml
  format: yaml
  label: Wikimedia offline API
  slug: wikimedia-offline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-offline-api-openapi.yml
- filename: wikimedia-page-content-api-openapi.yml
  format: yaml
  label: Wikimedia Page content API
  slug: wikimedia-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-page-content-api-openapi.yml
- filename: wikimedia-projects-api-openapi.yml
  format: yaml
  label: Wikimedia projects API
  slug: wikimedia-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-projects-api-openapi.yml
- filename: wikimedia-reading-lists-api-openapi.yml
  format: yaml
  label: Wikimedia Reading lists API
  slug: wikimedia-reading-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-reading-lists-api-openapi.yml
- filename: wikimedia-recommendation-api-openapi.yml
  format: yaml
  label: Wikimedia Recommendation API
  slug: wikimedia-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-recommendation-api-openapi.yml
- filename: wikimedia-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia snapshots API
  slug: wikimedia-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-snapshots-api-openapi.yml
- filename: wikimedia-structured-contents-api-openapi.yml
  format: yaml
  label: Wikimedia structured-contents API
  slug: wikimedia-structured-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-structured-contents-api-openapi.yml
- filename: wikimedia-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikimedia structured-snapshots API
  slug: wikimedia-structured-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-structured-snapshots-api-openapi.yml
- filename: wikimedia-talk-pages-api-openapi.yml
  format: yaml
  label: Wikimedia Talk pages API
  slug: wikimedia-talk-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-talk-pages-api-openapi.yml
- filename: wikimedia-transforms-api-openapi.yml
  format: yaml
  label: Wikimedia Transforms API
  slug: wikimedia-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-transforms-api-openapi.yml
- filename: wikimedia-wikidata-api-openapi.yml
  format: yaml
  label: Wikimedia wikidata API
  slug: wikimedia-wikidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-wikidata-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mediawiki.org
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: www.mediawiki.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: enterprise.wikimedia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wikimedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikimedia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wikimedia
provider_slug: wikimedia
slug: wikimedia-domain-security
source_filename: wikimedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mediawiki.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: enterprise.wikimedia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mediawiki.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/security/wikimedia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Wikipedia
- Wikimedia
- Encyclopedia
- Open Knowledge
- Content
- Search
- Reference
---
