---
api_specs:
- filename: flickr-openapi.yml
  format: yaml
  label: Flickr API
  slug: flickr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flickr/refs/heads/main/openapi/flickr-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "letsencrypt.org"
  - 0 iodef "mailto:hostmaster@smugmug.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: flickr.com
  spf: true
hosts:
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: www.flickr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: api.flickr.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  2 23:59:59 2027 GMT
  host: up.flickr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Flickr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flickr, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flickr
provider_slug: flickr
slug: flickr-domain-security
source_filename: flickr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.flickr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: api.flickr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: false\n- host: up.flickr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  2 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: flickr.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 iodef \"mailto:hostmaster@smugmug.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flickr/refs/heads/main/security/flickr-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Photography
- Photos
- Social Media
- Public APIs
---
