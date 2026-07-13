---
api_specs:
- filename: musixmatch-openapi-original.yml
  format: yaml
  label: Musixmatch API
  slug: musixmatch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/openapi/musixmatch-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "amazon.com"
  - 0 issue "globalsign.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: musixmatch.com
  spf: true
hosts:
- cert_expires: Sep 11 08:02:53 2026 GMT
  host: developer.musixmatch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
- cert_expires: Nov 26 16:00:13 2026 GMT
  host: api.musixmatch.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Musixmatch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Musixmatch, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Musixmatch
provider_slug: musixmatch
slug: musixmatch-domain-security
source_filename: musixmatch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.musixmatch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 11 08:02:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.musixmatch.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 16:00:13 2026 GMT\n  hsts: null\ndomains:\n- domain: musixmatch.com\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"globalsign.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"globalsign.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/musixmatch/refs/heads/main/security/musixmatch-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Lyrics
- Music
- Translations
---
