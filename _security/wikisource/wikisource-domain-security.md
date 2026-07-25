---
api_specs:
- filename: wikisource-citation-api-openapi.yml
  format: yaml
  label: Wikisource Citation API
  slug: wikisource-citation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-citation-api-openapi.yml
- filename: wikisource-math-api-openapi.yml
  format: yaml
  label: Wikisource Math API
  slug: wikisource-math-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-math-api-openapi.yml
- filename: wikisource-mobile-api-openapi.yml
  format: yaml
  label: Wikisource Mobile API
  slug: wikisource-mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-mobile-api-openapi.yml
- filename: wikisource-page-content-api-openapi.yml
  format: yaml
  label: Wikisource Page content API
  slug: wikisource-page-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-page-content-api-openapi.yml
- filename: wikisource-reading-lists-api-openapi.yml
  format: yaml
  label: Wikisource Reading lists API
  slug: wikisource-reading-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-reading-lists-api-openapi.yml
- filename: wikisource-recommendation-api-openapi.yml
  format: yaml
  label: Wikisource Recommendation API
  slug: wikisource-recommendation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-recommendation-api-openapi.yml
- filename: wikisource-transforms-api-openapi.yml
  format: yaml
  label: Wikisource Transforms API
  slug: wikisource-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikisource-transforms-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikisource.org
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mediawiki.org
  spf: true
hosts:
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: wikisource.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 20:06:43 2026 GMT
  host: en.wikisource.org
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
name: Wikisource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikisource, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wikisource
provider_slug: wikisource
slug: wikisource-domain-security
source_filename: wikisource-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wikisource.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: en.wikisource.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: www.mediawiki.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wikisource.org\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mediawiki.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/security/wikisource-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- Open Knowledge
- Literature
- Historical Documents
- Public Domain
- Transcription
- Primary Sources
- Non-Profit
- Open Source
---
