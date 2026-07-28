---
api_specs:
- filename: ferc-data-api-openapi.json
  format: json
  label: FERC Open Data API
  slug: ferc-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-data-api-openapi.json
- filename: ferc-eforms-api-openapi-derived.yml
  format: yaml
  label: FERC eForms XBRL Submission API
  slug: ferc-eforms-xbrl-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/openapi/ferc-eforms-api-openapi-derived.yml
description: ''
domains:
- caa:
  - 0 iodef "hostmaster@ferc.gov"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "digicert.com"
  - 0 issuewild "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ferc.gov
  spf: true
hosts:
- cert_expires: Oct 12 10:19:17 2026 GMT
  host: www.ferc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 23 15:14:32 2026 GMT
  host: data.ferc.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 24 18:21:24 2026 GMT
  cert_issuer: Let's Encrypt
  gateway: api.data.gov API Umbrella on cloud.gov
  host: api.data.ferc.gov
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'The automated probe recorded hsts null because the gateway answers HEAD / differently; a live GET on 2026-07-27 returned "strict-transport-security: max-age=31536000; includeSubDomains; preload". Corrected from the observed response.'
  hsts_preload: true
  https: true
  security_headers:
  - 'x-content-type-options: nosniff'
  - 'x-frame-options: DENY'
  - 'x-xss-protection: 1; mode=block'
  - 'access-control-allow-origin: *'
  tls_version: TLSv1.3
- cert_expires: Feb 11 23:59:59 2027 GMT
  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1
  host: ecollection.ferc.gov
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_preload: false
  https: true
  note: Added by hand — the eForms API base host was not covered by the automated probe. It is the only FERC host observed negotiating TLS 1.2 rather than 1.3, and its X-Frame-Options value ("ALLOW-FROM https://") is malformed and ignored by modern browsers; the CSP frame-ancestors directive is what actually protects it.
  probed: '2026-07-27'
  security_headers:
  - 'content-security-policy: frame-ancestors https://*.ferc.gov:*'
  - 'x-xss-protection: 1; mode=block'
  - 'x-frame-options: ALLOW-FROM https://'
  tls_cipher: ECDHE-RSA-AES256-GCM-SHA384
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ferc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FERC, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: FERC
provider_slug: ferc
slug: ferc-domain-security
source_filename: ferc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ferc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 10:19:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: data.ferc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 15:14:32 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.data.ferc.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 18:21:24 2026 GMT\n  cert_issuer: Let's Encrypt\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: true\n  hsts_note: >-\n    The automated probe recorded hsts null because the gateway answers HEAD / differently; a live\n    GET on 2026-07-27 returned \"strict-transport-security: max-age=31536000; includeSubDomains;\n    preload\". Corrected from the observed response.\n  security_headers:\n  - 'x-content-type-options: nosniff'\n  - 'x-frame-options: DENY'\n\
  \  - 'x-xss-protection: 1; mode=block'\n  - 'access-control-allow-origin: *'\n  gateway: api.data.gov API Umbrella on cloud.gov\n- host: ecollection.ferc.gov\n  https: true\n  tls_version: TLSv1.2\n  tls_cipher: ECDHE-RSA-AES256-GCM-SHA384\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  cert_issuer: DigiCert Global G2 TLS RSA SHA256 2020 CA1\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_preload: false\n  security_headers:\n  - 'content-security-policy: frame-ancestors https://*.ferc.gov:*'\n  - 'x-xss-protection: 1; mode=block'\n  - 'x-frame-options: ALLOW-FROM https://'\n  note: >-\n    Added by hand — the eForms API base host was not covered by the automated probe. It is the only\n    FERC host observed negotiating TLS 1.2 rather than 1.3, and its X-Frame-Options value\n    (\"ALLOW-FROM https://\") is malformed and ignored by modern browsers; the CSP frame-ancestors\n    directive is what actually protects it.\n  probed: '2026-07-27'\ndomains:\n- domain:\
  \ ferc.gov\n  dnssec: true\n  caa:\n  - 0 iodef \"hostmaster@ferc.gov\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"digicert.com\"\n  - 0 issuewild \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ferc/refs/heads/main/security/ferc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Energy
- United States
- Energy Markets
- Electricity
- Natural Gas
- Grid
- Regulator
- Government
- Open Data
- Wholesale Power Markets
- Hydropower
- Oil Pipelines
---
