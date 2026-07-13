---
api_specs:
- filename: wcv2
  format: yaml
  label: WorldCat Search API
  slug: worldcat-search-api
  spec_type: OpenAPI
  url: https://developer.api.oclc.org/wcv2
- filename: wc-metadata-v2
  format: yaml
  label: WorldCat Metadata API
  slug: worldcat-metadata-api
  spec_type: OpenAPI
  url: https://developer.api.oclc.org/wc-metadata-v2
- filename: worldcat-knowledge-base-api.yml
  format: yaml
  label: WorldCat Knowledge Base API
  slug: worldcat-knowledge-base-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/worldcat/refs/heads/main/openapi/worldcat-knowledge-base-api.yml
- filename: entity-data
  format: yaml
  label: WorldCat Entities Data API
  slug: worldcat-entities-data-api
  spec_type: OpenAPI
  url: https://developer.api.oclc.org/entity-data
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: worldcat.org
  spf: false
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 128 issue "amazon.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: oclc.org
  spf: true
hosts:
- cert_expires: Oct  5 02:44:56 2026 GMT
  host: www.worldcat.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 08:54:21 2026 GMT
  host: www.oclc.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 21:59:19 2026 GMT
  host: americas.discovery.api.oclc.org
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Worldcat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorldCat, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC present (p=quarantine).'
provider_name: WorldCat
provider_slug: worldcat
slug: worldcat-domain-security
source_filename: worldcat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.worldcat.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 02:44:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.oclc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 08:54:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: americas.discovery.api.oclc.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 21:59:19 2026 GMT\n  hsts: null\ndomains:\n- domain: worldcat.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: oclc.org\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\
  \n  - 0 issuewild \"ssl.com\"\n  - 128 issue \"amazon.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldcat/refs/heads/main/security/worldcat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Libraries
- Bibliographic Records
- WorldCat
- OCLC
- Cataloging
- Metadata
- Discovery
- Books
- Media
- Linked Data
---
