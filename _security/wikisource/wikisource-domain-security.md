---
api_specs:
- filename: wikimedia-rest-api-v1-openapi.json
  format: json
  label: Wikimedia REST API v1
  slug: wikimedia-rest-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wikisource/refs/heads/main/openapi/wikimedia-rest-api-v1-openapi.json
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
