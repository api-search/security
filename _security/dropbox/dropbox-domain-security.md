---
api_specs:
- filename: dropbox-openapi-original.yml
  format: yaml
  label: Dropbox API
  slug: dropbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox/refs/heads/main/openapi/dropbox-openapi-original.yml
- filename: dropbox-sign-openapi-original.yml
  format: yaml
  label: Dropbox Sign API
  slug: dropbox-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox/refs/heads/main/openapi/dropbox-sign-openapi-original.yml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dropbox.com
  spf: true
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dropboxapi.com
  spf: false
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: www.dropbox.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: api.dropboxapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 13:08:55 2026 GMT
  host: developers.hellosign.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dropbox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropbox, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dropbox
provider_slug: dropbox
slug: dropbox-domain-security
source_filename: dropbox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dropbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.dropboxapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\n- host: developers.hellosign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:08:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dropbox.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: dropboxapi.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\
  \n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropbox/refs/heads/main/security/dropbox-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Documents
---
