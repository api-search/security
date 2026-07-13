---
api_specs:
- filename: numlookupapi-openapi.yml
  format: yaml
  label: NumLookupAPI Phone Number Validation API
  slug: numlookupapi-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numlookupapi/refs/heads/main/openapi/numlookupapi-openapi.yml
- filename: numlookupapi-openapi.yml
  format: yaml
  label: NumLookupAPI Account Status API
  slug: numlookupapi-account-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/numlookupapi/refs/heads/main/openapi/numlookupapi-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: numlookupapi.com
  spf: true
  spf_record: v=spf1 include:spf.sendinblue.com include:spf.improvmx.com include:mail.zendesk.com mx ~all
hosts:
- cert_expires: Oct  7 06:44:54 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: numlookupapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: Netlify
  tls_version: TLSv1.3
- host: www.numlookupapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: Netlify
  tls_version: TLSv1.3
- cert_expires: Oct  7 06:44:54 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  gateway: Kong
  host: api.numlookupapi.com
  hsts: false
  https: true
  notes: Unauthenticated requests return HTTP/2 401 with WWW-Authenticate Key realm="kong". No Strict-Transport-Security header was returned on the API host at probe time.
  server: cloudflare
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Numlookupapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NumLookupAPI, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: NumLookupAPI
provider_slug: numlookupapi
slug: numlookupapi-domain-security
source_filename: numlookupapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: numlookupapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  7 06:44:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: Netlify\n- host: www.numlookupapi.com\n  https: true\n  tls_version: TLSv1.3\n  hsts: true\n  hsts_max_age: 31536000\n  server: Netlify\n- host: api.numlookupapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_issuer: Google Trust Services (WE1)\n  cert_expires: Oct  7 06:44:54 2026 GMT\n  hsts: false\n  server: cloudflare\n  gateway: Kong\n  notes: >-\n    Unauthenticated requests return HTTP/2 401 with WWW-Authenticate Key\n    realm=\"kong\". No Strict-Transport-Security header was returned on the API\n    host at probe time.\ndomains:\n- domain: numlookupapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:spf.sendinblue.com include:spf.improvmx.com\
  \ include:mail.zendesk.com mx ~all\n  dmarc: true\n  dmarc_policy: quarantine\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/numlookupapi/refs/heads/main/security/numlookupapi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Number Verification
- Phone Validation
- Phone Number Lookup
- Carrier Lookup
- Line Type
- Verification
- Data Validation
- Caller Identity
---
