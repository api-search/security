---
api_specs:
- filename: hellosign-openapi-original.yaml
  format: yaml
  label: Dropbox Sign API
  slug: dropbox-sign-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/openapi/hellosign-openapi-original.yaml
description: ''
domains:
- caa:
  - 0 issue "amazonaws.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hellosign.com
  spf: true
hosts:
- cert_expires: Oct 14 23:59:59 2026 GMT
  host: api.hellosign.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hellosign Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dropbox Sign (HelloSign), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Dropbox Sign (HelloSign)
provider_slug: hellosign
slug: hellosign-domain-security
source_filename: hellosign-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.hellosign.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: hellosign.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org;validationmethods=dns-01;accounturi=https://acme-v02.api.letsencrypt.org/acme/acct/2079416047\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hellosign/refs/heads/main/security/hellosign-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- eSignature
- Electronic Signatures
- Documents
- Digital Agreements
- Signature Workflow
- Embedded Signing
- Compliance
---
