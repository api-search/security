---
api_specs:
- filename: words-categories-api-openapi.yml
  format: yaml
  label: Words API Categories API
  slug: words-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-categories-api-openapi.yml
- filename: words-definitions-api-openapi.yml
  format: yaml
  label: Words API Definitions API
  slug: words-definitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-definitions-api-openapi.yml
- filename: words-examples-api-openapi.yml
  format: yaml
  label: Words API Examples API
  slug: words-examples-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-examples-api-openapi.yml
- filename: words-frequency-api-openapi.yml
  format: yaml
  label: Words API Frequency API
  slug: words-frequency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-frequency-api-openapi.yml
- filename: words-hierarchy-api-openapi.yml
  format: yaml
  label: Words API Hierarchy API
  slug: words-hierarchy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-hierarchy-api-openapi.yml
- filename: words-phonetics-api-openapi.yml
  format: yaml
  label: Words API Phonetics API
  slug: words-phonetics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-phonetics-api-openapi.yml
- filename: words-search-api-openapi.yml
  format: yaml
  label: Words API Search API
  slug: words-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-search-api-openapi.yml
- filename: words-thesaurus-api-openapi.yml
  format: yaml
  label: Words API Thesaurus API
  slug: words-thesaurus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-thesaurus-api-openapi.yml
- filename: words-word-api-openapi.yml
  format: yaml
  label: Words API Word API
  slug: words-word-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/openapi/words-word-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: wordsapi.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: rapidapi.com
  spf: true
hosts:
- cert_expires: Oct  4 21:58:58 2026 GMT
  host: www.wordsapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 23:59:59 2026 GMT
  host: wordsapiv1.p.rapidapi.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Words Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Words API, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Words API
provider_slug: words
slug: words-domain-security
source_filename: words-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wordsapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 21:58:58 2026 GMT\n  hsts: false\n- host: wordsapiv1.p.rapidapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: wordsapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: rapidapi.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/words/refs/heads/main/security/words-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Dictionaries
- Linguistics
- English
- thesaurus
- Lexical Data
- Public APIs
---
