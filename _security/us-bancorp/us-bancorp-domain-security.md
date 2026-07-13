---
api_specs:
- filename: us-bank-corporate-account-information-openapi.yml
  format: yaml
  label: US Bank Corporate Account Information API
  slug: us-bank-corporate-account-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-corporate-account-information-openapi.yml
- filename: us-bank-rtp-openapi.yml
  format: yaml
  label: US Bank RTP Real-Time Payments API
  slug: us-bank-rtp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-rtp-openapi.yml
- filename: us-bank-ach-originations-openapi.yml
  format: yaml
  label: US Bank ACH Originations API
  slug: us-bank-ach-originations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-ach-originations-openapi.yml
- filename: us-bank-positive-pay-openapi.yml
  format: yaml
  label: US Bank Positive Pay API
  slug: us-bank-positive-pay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-positive-pay-openapi.yml
- filename: us-bank-push-to-card-openapi.yml
  format: yaml
  label: US Bank Push to Card API
  slug: us-bank-push-to-card
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/openapi/us-bank-push-to-card-openapi.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:domainadmin@usbank.com"
  - 0 iodef "mailto:certificateservicesshared@usbank.com"
  - 0 issue "digicert.com"
  - 0 issue "entrust.net"
  - 0 issuewild ";"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: usbank.com
  spf: true
hosts:
- cert_expires: Feb  9 23:59:59 2027 GMT
  host: developer.usbank.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 12 23:59:59 2027 GMT
  host: api.usbank.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Us Bancorp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for US Bancorp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: US Bancorp
provider_slug: us-bancorp
slug: us-bancorp-domain-security
source_filename: us-bancorp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.usbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  9 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.usbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 12 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: usbank.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:domainadmin@usbank.com\"\n  - 0 iodef \"mailto:certificateservicesshared@usbank.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"entrust.net\"\n  - 0 issuewild \";\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-bancorp/refs/heads/main/security/us-bancorp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Banking
- Finance
- Fortune 500
- Corporate Banking
- Payments
- Open Banking
- Treasury Management
- Consumer Banking
---
