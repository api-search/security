---
api_specs:
- filename: freepik-audio-api-openapi.yml
  format: yaml
  label: Freepik Audio API
  slug: freepik-audio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-audio-api-openapi.yml
- filename: freepik-image-editing-api-openapi.yml
  format: yaml
  label: Freepik Image Editing API
  slug: freepik-image-editing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-image-editing-api-openapi.yml
- filename: freepik-image-generation-api-openapi.yml
  format: yaml
  label: Freepik Image Generation API
  slug: freepik-image-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-image-generation-api-openapi.yml
- filename: freepik-resources-api-openapi.yml
  format: yaml
  label: Freepik Resources API
  slug: freepik-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-resources-api-openapi.yml
- filename: freepik-tasks-api-openapi.yml
  format: yaml
  label: Freepik Tasks API
  slug: freepik-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-tasks-api-openapi.yml
- filename: freepik-video-generation-api-openapi.yml
  format: yaml
  label: Freepik Video Generation API
  slug: freepik-video-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/openapi/freepik-video-generation-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: freepik.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "sectigo.com"
  - 0 issuewild "pki.goog"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: magnific.com
  spf: true
hosts:
- cert_expires: Sep  2 01:22:02 2026 GMT
  host: www.freepik.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 16:55:11 2026 GMT
  host: docs.freepik.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 17:35:09 2026 GMT
  host: api.magnific.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Freepik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freepik, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Freepik
provider_slug: freepik
slug: freepik-domain-security
source_filename: freepik-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.freepik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 01:22:02 2026 GMT\n  hsts: null\n- host: docs.freepik.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 16:55:11 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.magnific.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:35:09 2026 GMT\n  hsts: null\ndomains:\n- domain: freepik.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: magnific.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"sectigo.com\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issue \"letsencrypt.org\"\
  \n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freepik/refs/heads/main/security/freepik-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Graphics
- Illustrations
- Image Generation
- Photos
- Video Generation
---
