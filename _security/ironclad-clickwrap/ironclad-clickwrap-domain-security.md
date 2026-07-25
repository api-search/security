---
api_specs:
- filename: ironclad-clickwrap-activity-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Activity API
  slug: ironclad-clickwrap-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-activity-api-openapi.yml
- filename: ironclad-clickwrap-contracts-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Contracts API
  slug: ironclad-clickwrap-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-contracts-api-openapi.yml
- filename: ironclad-clickwrap-groups-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Groups API
  slug: ironclad-clickwrap-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-groups-api-openapi.yml
- filename: ironclad-clickwrap-signers-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Signers API
  slug: ironclad-clickwrap-signers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-signers-api-openapi.yml
- filename: ironclad-clickwrap-sites-api-openapi.yml
  format: yaml
  label: Ironclad Clickwrap Sites API
  slug: ironclad-clickwrap-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/openapi/ironclad-clickwrap-sites-api-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:security@ironcladhq.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "digicert.com"
  - 0 issue "comodoca.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ironcladapp.com
  spf: true
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:security@ironcladhq.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: pactsafe.io
  spf: true
hosts:
- cert_expires: Aug 14 21:17:12 2026 GMT
  host: clickwrap-developer.ironcladapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 18 17:57:51 2026 GMT
  host: ironcladapp.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 28 23:59:59 2026 GMT
  host: pactsafe.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Ironclad Clickwrap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ironclad Clickwrap, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ironclad Clickwrap
provider_slug: ironclad-clickwrap
slug: ironclad-clickwrap-domain-security
source_filename: ironclad-clickwrap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: clickwrap-developer.ironcladapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 21:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ironcladapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 17:57:51 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: pactsafe.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ironcladapp.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:security@ironcladhq.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: pactsafe.io\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:security@ironcladhq.com\"\
  \n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ironclad-clickwrap/refs/heads/main/security/ironclad-clickwrap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Agreements
- Compliance
- Contracts
- Legal
---
