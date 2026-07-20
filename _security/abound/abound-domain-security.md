---
api_specs:
- filename: abound-v4-openapi.yml
  format: yaml
  label: Abound API v4
  slug: abound-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/openapi/abound-v4-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: withabound.com
  spf: false
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: npmjs.com
  spf: true
hosts:
- host: withabound.com
  https: false
- cert_expires: Oct 12 04:22:28 2026 GMT
  host: www.npmjs.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: production-api.withabound.com
  https: false
kind: domain-security
layout: security
method: probed
name: Abound Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abound, probed live across 3 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Abound
provider_slug: abound
slug: abound-domain-security
source_filename: abound-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nnote: >-\n  The withabound.com zone has no delegated nameservers, so every withabound.com host is NXDOMAIN\n  and the negative results below (no HTTPS, no DNSSEC, no CAA, no SPF, no DMARC) reflect a retired\n  service rather than a weak security posture. www.npmjs.com appears only because the surviving\n  first-party SDK is the API's humanURL. See lifecycle/abound-lifecycle.yml.\nhosts:\n- host: withabound.com\n  https: false\n- host: www.npmjs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 04:22:28 2026 GMT\n  hsts: null\n- host: production-api.withabound.com\n  https: false\ndomains:\n- domain: withabound.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: npmjs.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n\
  \  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abound/refs/heads/main/security/abound-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Taxes
- Tax Compliance
- Regulatory Compliance
- Financial Services
- Identity Verification
- Government
- Documents
- Webhooks
- Retired
---
