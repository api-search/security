---
api_specs:
- filename: sofi-technologies-program-api-openapi.json
  format: json
  label: SoFi Tech Solutions Program API
  slug: sofi-tech-solutions-program-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-program-api-openapi.json
- filename: sofi-technologies-payment-hub-api-openapi.json
  format: json
  label: SoFi Tech Solutions Payment Hub API 2.0
  slug: sofi-tech-solutions-payment-hub-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-payment-hub-api-openapi.json
- filename: sofi-technologies-dispute-api-3-0-openapi.json
  format: json
  label: SoFi Tech Solutions Dispute API 3.0
  slug: sofi-tech-solutions-dispute-api-30
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-dispute-api-3-0-openapi.json
- filename: sofi-technologies-dispute-api-2-0-openapi.json
  format: json
  label: SoFi Tech Solutions Dispute API 2.0
  slug: sofi-tech-solutions-dispute-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-dispute-api-2-0-openapi.json
- filename: sofi-technologies-loan-api-openapi.json
  format: json
  label: SoFi Tech Solutions Loan API
  slug: sofi-tech-solutions-loan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-loan-api-openapi.json
- filename: sofi-technologies-risk-api-2-0-openapi.json
  format: json
  label: SoFi Tech Solutions Risk API 2.0
  slug: sofi-tech-solutions-risk-api-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-risk-api-2-0-openapi.json
- filename: sofi-technologies-risk-api-1-0-openapi.json
  format: json
  label: SoFi Tech Solutions Risk API 1.0
  slug: sofi-tech-solutions-risk-api-10
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-risk-api-1-0-openapi.json
- filename: sofi-technologies-public-config-api-openapi.json
  format: json
  label: SoFi Tech Solutions Public Config API
  slug: sofi-tech-solutions-public-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-public-config-api-openapi.json
- filename: sofi-technologies-events-api-openapi.json
  format: json
  label: SoFi Tech Solutions Events API
  slug: sofi-tech-solutions-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-events-api-openapi.json
- filename: sofi-technologies-auth-api-openapi.json
  format: json
  label: SoFi Tech Solutions Auth API
  slug: sofi-tech-solutions-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-auth-api-openapi.json
- filename: sofi-technologies-external-trans-api-openapi.json
  format: json
  label: SoFi Tech Solutions External Trans API
  slug: sofi-tech-solutions-external-trans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/openapi/sofi-technologies-external-trans-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "globalsign.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sofi.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gpsrv.com
  note: The legacy Galileo processing domain that still hosts every API server template. DMARC is p=none - monitor only, no enforcement - on the domain that carries the platform's entire callable surface, while sofi.com itself is at p=reject. Mail is behind Proofpoint.
  spf: true
hosts:
- cert_expires: Dec  8 23:40:23 2026 GMT
  host: www.sofi.com
  hsts: null
  https: true
  note: Answers 403 to any non-browser client (Cloudflare bot challenge) while serving a real 317 KB page. Live, not dead.
  tls_version: TLSv1.3
- cert_expires: Oct  8 22:20:35 2026 GMT
  host: tech.sofi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 00:06:15 2026 GMT
  host: docs.tech.sofi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  8 23:40:23 2026 GMT
  host: api.sofi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  note: Live nginx behind Cloudflare; every probed path returns 404. No public contract here.
  tls_version: TLSv1.3
- cert_expires: Oct 18 02:13:14 2026 GMT
  host: sandbox.gpsrv.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 63072000
  https: true
  note: The Sandbox dashboard where clients read their Sandbox API connection details.
  tls_version: TLSv1.3
- host: sandbox-api.gpsrv.com
  https: unknown
  note: TCP connect times out from an arbitrary source. The Sandbox API host is IP-allowlisted, which is consistent with credentials being bound to a registered requesting IP.
- host: developer.sofi.com
  https: false
  note: NXDOMAIN. This host was the humanURL on this record before 2026-09-06 and never existed; the pointer has been removed.
hosts_probed: 7
kind: domain-security
layout: security
method: probed
name: Sofi Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SoFi Technologies, probed live across 7 host(s) and 2 registrable domain(s). 6 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SoFi Technologies
provider_slug: sofi-technologies
slug: sofi-technologies-domain-security
source_filename: sofi-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  live DNS/TLS/HTTP probes of the hosts this record names, run by\n  0-working/probe-domain-security.py and then hand-corrected to drop two rows the script derived\n  from placeholder server values - see excluded below.\nhosts:\n  - host: www.sofi.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Dec  8 23:40:23 2026 GMT\n    hsts: null\n    note: >-\n      Answers 403 to any non-browser client (Cloudflare bot challenge) while serving a real 317 KB\n      page. Live, not dead.\n  - host: tech.sofi.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct  8 22:20:35 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n  - host: docs.tech.sofi.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct 13 00:06:15 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n  - host: api.sofi.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires:\
  \ Dec  8 23:40:23 2026 GMT\n    hsts: true\n    hsts_max_age: 31536000\n    hsts_include_subdomains: true\n    note: Live nginx behind Cloudflare; every probed path returns 404. No public contract here.\n  - host: sandbox.gpsrv.com\n    https: true\n    tls_version: TLSv1.3\n    cert_expires: Oct 18 02:13:14 2026 GMT\n    hsts: true\n    hsts_max_age: 63072000\n    hsts_include_subdomains: true\n    note: The Sandbox dashboard where clients read their Sandbox API connection details.\n  - host: sandbox-api.gpsrv.com\n    https: unknown\n    note: >-\n      TCP connect times out from an arbitrary source. The Sandbox API host is IP-allowlisted, which\n      is consistent with credentials being bound to a registered requesting IP.\n  - host: developer.sofi.com\n    https: false\n    note: >-\n      NXDOMAIN. This host was the humanURL on this record before 2026-09-06 and never existed; the\n      pointer has been removed.\ndomains:\n  - domain: sofi.com\n    dnssec: false\n    caa:\n     \
  \ - 0 issue \"pki.goog\"\n      - 0 issue \"amazon.com\"\n      - 0 issuewild \"amazon.com\"\n      - 0 issuewild \"globalsign.com\"\n      - 0 issuewild \"godaddy.com\"\n      - 0 issuewild \"pki.goog\"\n    spf: true\n    dmarc: true\n    dmarc_policy: reject\n  - domain: gpsrv.com\n    dnssec: false\n    caa: []\n    spf: true\n    dmarc: true\n    dmarc_policy: none\n    note: >-\n      The legacy Galileo processing domain that still hosts every API server template. DMARC is\n      p=none - monitor only, no enforcement - on the domain that carries the platform's entire\n      callable surface, while sofi.com itself is at p=reject. Mail is behind Proofpoint.\nexcluded:\n  - value: client.domain.com\n    reason: >-\n      Not a SoFi host. It is the placeholder server in the Events API and External Trans API\n      contracts, where the CLIENT hosts the endpoint. The automated probe treated it as a real\n      host and would have recorded a third party's SPF and DMARC posture as SoFi's.\n\
  \  - value: example.client.domain.com\n    reason: Same - the Auth API's client-hosted placeholder server.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sofi-technologies/refs/heads/main/security/sofi-technologies-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- Payments
- Banking
- Card Issuing
- Banking as a Service
- Personal Finance
- Lending
- ACH
- ISO 20022
- Disputes
- Identity Verification
- Webhooks
---
