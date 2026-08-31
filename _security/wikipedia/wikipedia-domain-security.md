---
api_specs:
- filename: wikipedia-articles-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki articles API
  slug: wikipedia-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-articles-api-openapi.yml
- filename: wikipedia-batches-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki batches API
  slug: wikipedia-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-batches-api-openapi.yml
- filename: wikipedia-citation-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Citation API
  slug: wikipedia-citation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-citation-api-openapi.yml
- filename: wikipedia-codes-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki codes API
  slug: wikipedia-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-codes-api-openapi.yml
- filename: wikipedia-languages-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki languages API
  slug: wikipedia-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-languages-api-openapi.yml
- filename: wikipedia-math-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Math API
  slug: wikipedia-math-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-math-api-openapi.yml
- filename: wikipedia-mobile-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Mobile API
  slug: wikipedia-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-mobile-api-openapi.yml
- filename: wikipedia-namespaces-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki namespaces API
  slug: wikipedia-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-namespaces-api-openapi.yml
- filename: wikipedia-offline-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki offline API
  slug: wikipedia-offline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-offline-api-openapi.yml
- filename: wikipedia-page-content-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Page content API
  slug: wikipedia-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-page-content-api-openapi.yml
- filename: wikipedia-projects-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki projects API
  slug: wikipedia-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-projects-api-openapi.yml
- filename: wikipedia-reading-lists-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Reading lists API
  slug: wikipedia-reading-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-reading-lists-api-openapi.yml
- filename: wikipedia-recommendation-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Recommendation API
  slug: wikipedia-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-recommendation-api-openapi.yml
- filename: wikipedia-snapshots-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki snapshots API
  slug: wikipedia-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-snapshots-api-openapi.yml
- filename: wikipedia-structured-contents-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki structured-contents API
  slug: wikipedia-structured-contents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-structured-contents-api-openapi.yml
- filename: wikipedia-structured-snapshots-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki structured-snapshots API
  slug: wikipedia-structured-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-structured-snapshots-api-openapi.yml
- filename: wikipedia-talk-pages-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Talk pages API
  slug: wikipedia-talk-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-talk-pages-api-openapi.yml
- filename: wikipedia-transforms-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki Transforms API
  slug: wikipedia-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-transforms-api-openapi.yml
- filename: wikipedia-wikidata-api-openapi.yml
  format: yaml
  label: Wikipedia / MediaWiki wikidata API
  slug: wikipedia-wikidata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/openapi/wikipedia-wikidata-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikipedia.org
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
  host: www.wikipedia.org
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
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikipedia.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wikipedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikipedia / MediaWiki, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wikipedia / MediaWiki
provider_slug: wikipedia
slug: wikipedia-domain-security
source_filename: wikipedia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: www.mediawiki.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: en.wikipedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wikipedia.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mediawiki.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikipedia/refs/heads/main/security/wikipedia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- Public APIs
- Open Knowledge
- Encyclopedia
- Knowledge Graph
- Open-Source
- Non-Profit
---
