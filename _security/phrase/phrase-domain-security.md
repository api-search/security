---
api_specs:
- filename: phrase-strings-openapi-original.yaml
  format: yaml
  label: Phrase Strings API
  slug: phrase-strings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/phrase/refs/heads/main/openapi/phrase-strings-openapi-original.yaml
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 iodef "mailto:security@memsource.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: phrase.com
  spf: true
hosts:
- cert_expires: Sep 15 08:49:36 2026 GMT
  host: developers.phrase.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 07:11:43 2026 GMT
  host: phrase.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: api.phrase.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Phrase Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Phrase, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Phrase
provider_slug: phrase
slug: phrase-domain-security
source_filename: phrase-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developers.phrase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 08:49:36 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: phrase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 07:11:43 2026 GMT\n  hsts: false\n- host: api.phrase.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: phrase.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 iodef \"mailto:security@memsource.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/phrase/refs/heads/main/security/phrase-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Content Management
- Localization
- Translation
- Strings
- Internationalization
---
