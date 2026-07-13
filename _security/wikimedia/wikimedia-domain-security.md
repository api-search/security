---
api_specs:
- filename: api.php
  format: yaml
  label: MediaWiki Action API
  slug: mediawiki-action-api
  spec_type: OpenAPI
  url: https://en.wikipedia.org/w/api.php?action=openapi
- filename: wikimedia-rest-api.json
  format: json
  label: Wikimedia REST API (RESTBase)
  slug: wikimedia-rest-api-restbase
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-rest-api.json
- filename: wikimedia-enterprise-api.yaml
  format: yaml
  label: Wikimedia Enterprise API
  slug: wikimedia-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikimedia/refs/heads/main/openapi/wikimedia-enterprise-api.yaml
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
