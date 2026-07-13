---
api_specs:
- filename: gopuff-fulfillment-openapi.yml
  format: yaml
  label: Powered by Gopuff Fulfillment API
  slug: fulfillment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/openapi/gopuff-fulfillment-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issue "pki.goog"
  - 0 issuewild "pki.goog"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gopuff.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: poweredbygopuff.com
  spf: false
hosts:
- cert_expires: Aug 27 12:20:09 2026 GMT
  host: www.gopuff.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 19 18:32:11 2026 GMT
  host: docs.poweredbygopuff.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 24 01:32:15 2026 GMT
  host: fulfillment-api-eus.partners.gopuff.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gopuff Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gopuff, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gopuff
provider_slug: gopuff
slug: gopuff-domain-security
source_filename: gopuff-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gopuff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 12:20:09 2026 GMT\n  hsts: null\n- host: docs.poweredbygopuff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 18:32:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: fulfillment-api-eus.partners.gopuff.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 01:32:15 2026 GMT\n  hsts: false\ndomains:\n- domain: gopuff.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"pki.goog\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: poweredbygopuff.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gopuff/refs/heads/main/security/gopuff-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Quick Commerce
- Instant Delivery
- Last Mile
- Grocery
- Fulfillment
- Retail
- Logistics
---
