---
api_specs:
- filename: swagger
  format: yaml
  label: Getty Images API
  slug: platform
  spec_type: OpenAPI
  url: https://api.gettyimages.com/swagger
description: ''
domains:
- caa:
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:dnsadmins@gettyimages.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: gettyimages.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.gettyimages.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 10 23:59:59 2027 GMT
  host: developer.gettyimages.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: api.gettyimages.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Getty Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Getty Images, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Getty Images
provider_slug: getty
slug: getty-domain-security
source_filename: getty-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gettyimages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: developer.gettyimages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.gettyimages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gettyimages.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:dnsadmins@gettyimages.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getty/refs/heads/main/security/getty-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stock Media
- Images
- Editorial
- Video
- Music
- Licensing
---
