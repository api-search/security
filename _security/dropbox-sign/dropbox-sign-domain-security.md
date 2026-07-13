---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Dropbox Sign REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://github.com/hellosign/hellosign-openapi/blob/main/openapi.yaml
- filename: dropbox-sign-events-asyncapi.yml
  format: yaml
  label: Dropbox Sign Events and Callbacks API
  slug: events-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dropbox-sign/refs/heads/main/asyncapi/dropbox-sign-events-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dropbox.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  - 0 issue "amazonaws.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hellosign.com
  spf: true
hosts:
- cert_expires: Dec 10 23:59:59 2026 GMT
  host: sign.dropbox.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 13:08:55 2026 GMT
  host: developers.hellosign.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.hellosign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dropbox Sign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropbox Sign, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dropbox Sign
provider_slug: dropbox-sign
slug: dropbox-sign-domain-security
source_filename: dropbox-sign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sign.dropbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 23:59:59 2026 GMT\n  hsts: false\n- host: developers.hellosign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 13:08:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.hellosign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dropbox.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hellosign.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\
  \n  - 0 issue \"amazonaws.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dropbox-sign/refs/heads/main/security/dropbox-sign-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- eSignature
- Electronic Signature
- Document Signing
- Workflow Automation
- Documents
---
