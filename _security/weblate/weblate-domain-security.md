---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Weblate REST API
  slug: weblate-rest-api
  spec_type: OpenAPI
  url: https://hosted.weblate.org/api/schema/
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: weblate.org
  spf: true
hosts:
- cert_expires: Sep 11 10:50:08 2026 GMT
  host: weblate.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 13:00:28 2026 GMT
  host: docs.weblate.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 19:47:44 2026 GMT
  host: hosted.weblate.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weblate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weblate, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Weblate
provider_slug: weblate
slug: weblate-domain-security
source_filename: weblate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weblate.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 10:50:08 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.weblate.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 13:00:28 2026 GMT\n  hsts: false\n- host: hosted.weblate.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 19:47:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: weblate.org\n  dnssec: true\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weblate/refs/heads/main/security/weblate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Localization
- Translation
- Internationalization
- Open Source
- Continuous Localization
- Version Control
---
