---
api_specs:
- filename: tyntec-number-verification-openapi.yml
  format: yaml
  label: tyntec Number Verification API
  slug: tyntec-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/openapi/tyntec-number-verification-openapi.yml
- filename: tyntec-number-verification-openapi.yml
  format: yaml
  label: tyntec Number Information API
  slug: tyntec-number-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/openapi/tyntec-number-verification-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_policy: reject
  domain: tyntec.com
  spf: true
  spf_record: v=spf1 mx include:aspmx.pardot.com -all
hosts:
- cert_expires: Sep  4 13:32:03 2026 GMT
  host: www.tyntec.com
  hsts: false
  http_status: 200
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 16 13:16:59 2027 GMT
  host: api.tyntec.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15552000
  http_status: 404
  https: true
  note: Root of api host returns 404; documented API paths (e.g. /verify/v1, /messaging/v1) are the live surface.
  tls_version: TLSv1.3
- cert_expires: Jan 16 13:16:59 2027 GMT
  host: tyntec.com
  http_status: 301
  https: true
  note: Redirects to www.tyntec.com.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tyntec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for tyntec, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: tyntec
provider_slug: tyntec
slug: tyntec-domain-security
source_filename: tyntec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tyntec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 13:32:03 2026 GMT\n  hsts: false\n  http_status: 200\n- host: api.tyntec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 13:16:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n  hsts_include_subdomains: true\n  http_status: 404\n  note: Root of api host returns 404; documented API paths (e.g. /verify/v1, /messaging/v1) are the live surface.\n- host: tyntec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 13:16:59 2027 GMT\n  http_status: 301\n  note: Redirects to www.tyntec.com.\ndomains:\n- domain: tyntec.com\n  dmarc: true\n  dmarc_policy: reject\n  spf: true\n  spf_record: v=spf1 mx include:aspmx.pardot.com -all\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tyntec/refs/heads/main/security/tyntec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Number Verification
- CPaaS
- SMS
- WhatsApp
- Phone Number Intelligence
- HLR Lookup
- Two-Factor Authentication
- OTP
- Messaging
- Number Portability
---
