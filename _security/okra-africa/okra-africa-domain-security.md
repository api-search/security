---
api_specs:
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Auth API
  slug: okra-africa-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Accounts API
  slug: okra-africa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Balance API
  slug: okra-africa-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Transactions API
  slug: okra-africa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Identity API
  slug: okra-africa-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Income API
  slug: okra-africa-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Verification (KYC) API
  slug: okra-africa-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Payments API
  slug: okra-africa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Banks API
  slug: okra-africa-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Customers API
  slug: okra-africa-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Wallet API
  slug: okra-africa-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Reports API
  slug: okra-africa-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: okra.ng
  mx: smtp.google.com
  nameservers:
  - nsa.whogohost.com
  - nsb.whogohost.com
  note: SPF and Google MX present on the parked domain; no DMARC or CAA. Reflects the current (post-Okra) registrant configuration, not Okra's original security posture.
  spf: true
  spf_record: v=spf1 +a +mx include:_spf.google.com include:relay.mailchannels.net ~all
hosts:
- host: okra.ng
  hosting: HostPapa (AS36352)
  hsts: false
  http_status: 500
  https: true
  https_valid: false
  ip: 23.94.150.194
  note: Parked / repurposed WordPress page; certificate belongs to an unrelated domain. Not operated by Okra.
  ptr: wgh22.wghservers.com
  resolves: true
  server: Apache
  tls_cert_cn: fggcowerrioga.com
  tls_cert_expired: true
  tls_cert_issuer: Let's Encrypt (R3)
  tls_cert_not_after: Jul 19 2023
- host: api.okra.ng
  note: NXDOMAIN - former production API base (https://api.okra.ng/v2). Dead.
  resolves: false
- host: dash.okra.ng
  note: NXDOMAIN - former developer dashboard / API key management. Dead.
  resolves: false
- host: docs.okra.ng
  note: NXDOMAIN - former API documentation. Archived on the Wayback Machine only.
  resolves: false
- host: identity-api.okra.ng
  note: NXDOMAIN - former Identity product host. Dead.
  resolves: false
kind: domain-security
layout: security
method: probed
name: Okra Africa Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Okra, probed live across 5 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Okra
provider_slug: okra-africa
slug: okra-africa-domain-security
source_filename: okra-africa-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of okra.ng and former Okra API/dev hosts\nstatus: retired\nretirementNote: >-\n  Okra ceased operations in May 2025. Live probes on 2026-07-12 confirm the\n  company's API and developer infrastructure is gone: api.okra.ng, dash.okra.ng,\n  docs.okra.ng, and identity-api.okra.ng do not resolve (NXDOMAIN). The apex\n  okra.ng now resolves to a HostPapa shared-hosting IP (23.94.150.194,\n  wgh22.wghservers.com) on whogohost nameservers and returns a broken/parked\n  WordPress page (HTTP 500 \"Requirements Not Met\"), presenting an EXPIRED Let's\n  Encrypt certificate issued to an unrelated domain (CN=fggcowerrioga.com,\n  expired 2023-07-19). This indicates the domain is no longer controlled/served\n  by Okra. Treat all former endpoints as dead.\nhosts:\n- host: okra.ng\n  resolves: true\n  ip: 23.94.150.194\n  ptr: wgh22.wghservers.com\n  hosting: HostPapa (AS36352)\n  https: true\n  https_valid: false\n\
  \  tls_cert_cn: fggcowerrioga.com\n  tls_cert_issuer: Let's Encrypt (R3)\n  tls_cert_expired: true\n  tls_cert_not_after: 'Jul 19 2023'\n  http_status: 500\n  server: Apache\n  hsts: false\n  note: Parked / repurposed WordPress page; certificate belongs to an unrelated domain. Not operated by Okra.\n- host: api.okra.ng\n  resolves: false\n  note: NXDOMAIN - former production API base (https://api.okra.ng/v2). Dead.\n- host: dash.okra.ng\n  resolves: false\n  note: NXDOMAIN - former developer dashboard / API key management. Dead.\n- host: docs.okra.ng\n  resolves: false\n  note: NXDOMAIN - former API documentation. Archived on the Wayback Machine only.\n- host: identity-api.okra.ng\n  resolves: false\n  note: NXDOMAIN - former Identity product host. Dead.\ndomains:\n- domain: okra.ng\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 +a +mx include:_spf.google.com include:relay.mailchannels.net ~all\n  dmarc: false\n  mx: smtp.google.com\n  nameservers:\n  - nsa.whogohost.com\n\
  \  - nsb.whogohost.com\n  note: SPF and Google MX present on the parked domain; no DMARC or CAA. Reflects the current (post-Okra) registrant configuration, not Okra's original security posture.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/security/okra-africa-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Open Banking
- Open Finance
- Financial Data
- Payments
- Fintech
- Account Linking
- Bank Data
- Africa
- Nigeria
- Financial Infrastructure
- Retired
---
