---
api_specs:
- filename: staples-advantage-eprocurement-api-openapi.yml
  format: yaml
  label: Staples Advantage eProcurement API
  slug: staples-advantage-eprocurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/staples/refs/heads/main/openapi/staples-advantage-eprocurement-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 iodef "mailto:ecams@staples.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: staples.com
  spf: true
- caa:
  - 0 iodef "mailto:ecams@staples.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: staplesadvantage.com
  spf: true
hosts:
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: www.staples.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 31 23:59:59 2026 GMT
  host: www.staplesadvantage.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: api.staplesadvantage.com
  hsts: null
  https: true
  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch, certificate is not valid for ''api.staples'
kind: domain-security
layout: security
method: probed
name: Staples Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Staples, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Staples
provider_slug: staples
slug: staples-domain-security
source_filename: staples-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.staples.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\n- host: www.staplesadvantage.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 23:59:59 2026 GMT\n  hsts: null\n- host: api.staplesadvantage.com\n  https: true\n  tls_cert_error: '[SSL: CERTIFICATE_VERIFY_FAILED] certificate verify failed: Hostname mismatch,\n    certificate is not valid for ''api.staples'\n  hsts: null\ndomains:\n- domain: staples.com\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:ecams@staples.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: staplesadvantage.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:ecams@staples.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy:\
  \ reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/staples/refs/heads/main/security/staples-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Office Supplies
- Retail
- Procurement
- B2B
- eProcurement
- Fortune 500
---
