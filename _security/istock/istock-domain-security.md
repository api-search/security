---
api_specs:
- filename: swagger
  format: yaml
  label: iStock API (Getty Platform)
  slug: platform
  spec_type: OpenAPI
  url: https://api.gettyimages.com/swagger
description: ''
domains:
- caa:
  - 0 iodef "mailto:dnsadmins@gettyimages.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "globalsign.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: istockphoto.com
  spf: true
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
- cert_expires: Dec 31 23:59:59 2026 GMT
  host: www.istockphoto.com
  hsts: true
  hsts_max_age: 2592000
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
name: Istock Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iStock, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: iStock
provider_slug: istock
slug: istock-domain-security
source_filename: istock-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.istockphoto.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.gettyimages.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: istockphoto.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:dnsadmins@gettyimages.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: gettyimages.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:dnsadmins@gettyimages.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"globalsign.com\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/security/istock-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stock Media
- Images
- Video
- Illustrations
- Royalty-Free
- Getty
---
