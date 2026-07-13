---
api_specs:
- filename: wikivoyage-mediawiki-action-api-openapi.yaml
  format: yaml
  label: Wikivoyage MediaWiki Action API
  slug: wikivoyage-mediawiki-action-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-mediawiki-action-api-openapi.yaml
- filename: wikivoyage-mediawiki-core-rest-openapi.yaml
  format: yaml
  label: Wikivoyage MediaWiki Core REST API
  slug: wikivoyage-mediawiki-core-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikivoyage/refs/heads/main/openapi/wikivoyage-mediawiki-core-rest-openapi.yaml
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
