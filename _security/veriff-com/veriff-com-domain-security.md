---
api_specs:
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Sessions API
  slug: veriff-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Decisions API
  slug: veriff-decisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Person API
  slug: veriff-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Media API
  slug: veriff-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Watchlist Screening API
  slug: veriff-watchlist-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Attempts API
  slug: veriff-attempts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
- filename: veriff-com-openapi.yml
  format: yaml
  label: Veriff Webhooks API
  slug: veriff-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/openapi/veriff-com-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "sectigo.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: veriff.com
  spf: true
hosts:
- cert_expires: Sep  8 05:27:02 2026 GMT
  host: www.veriff.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 09:58:46 2026 GMT
  host: devdocs.veriff.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: stationapi.veriff.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Veriff Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veriff, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Veriff
provider_slug: veriff-com
slug: veriff-com-domain-security
source_filename: veriff-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veriff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 05:27:02 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\n- host: devdocs.veriff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 09:58:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stationapi.veriff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: veriff.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veriff-com/refs/heads/main/security/veriff-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Identity Verification
- KYC
- AML
- Biometrics
- Document Verification
- Fraud Prevention
---
