---
api_specs:
- filename: wikidata-descriptions-api-openapi.yml
  format: yaml
  label: Wikidata Descriptions API
  slug: wikidata-descriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/openapi/wikidata-descriptions-api-openapi.yml
- filename: wikidata-items-api-openapi.yml
  format: yaml
  label: Wikidata Items API
  slug: wikidata-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/openapi/wikidata-items-api-openapi.yml
- filename: wikidata-labels-api-openapi.yml
  format: yaml
  label: Wikidata Labels API
  slug: wikidata-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/openapi/wikidata-labels-api-openapi.yml
- filename: wikidata-properties-api-openapi.yml
  format: yaml
  label: Wikidata Properties API
  slug: wikidata-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/openapi/wikidata-properties-api-openapi.yml
- filename: wikidata-statements-api-openapi.yml
  format: yaml
  label: Wikidata Statements API
  slug: wikidata-statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/openapi/wikidata-statements-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:dns-admin@wikimedia.org"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wikidata.org
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
  host: www.wikidata.org
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
  host: query.wikidata.org
  hsts: true
  hsts_max_age: 106384710
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wikidata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wikidata, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wikidata
provider_slug: wikidata
slug: wikidata-domain-security
source_filename: wikidata-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wikidata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: www.mediawiki.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\n- host: query.wikidata.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 20:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 106384710\ndomains:\n- domain: wikidata.org\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mediawiki.org\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:dns-admin@wikimedia.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wikidata/refs/heads/main/security/wikidata-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Knowledge Graph
- Linked Data
- Open Data
- Semantic Web
- SPARQL
- Wikipedia
---
