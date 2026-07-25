---
api_specs:
- filename: obie-opendata-standard.json
  format: json
  label: Paragon Bank Open Data API (OBIE standard, unverified)
  slug: paragon-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-opendata-standard.json
- filename: obie-account-info-standard.yaml
  format: yaml
  label: Paragon Bank Account and Transaction Information API (OBIE standard, unverified)
  slug: paragon-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-account-info-standard.yaml
- filename: obie-payment-initiation-standard.yaml
  format: yaml
  label: Paragon Bank Payment Initiation API (OBIE standard, unverified)
  slug: paragon-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-payment-initiation-standard.yaml
- filename: obie-confirmation-funds-standard.yaml
  format: yaml
  label: Paragon Bank Confirmation of Funds API (OBIE standard, unverified)
  slug: paragon-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/openapi/obie-confirmation-funds-standard.yaml
description: ''
domains:
- caa:
  - 0 issue "digicert.com"
  - 0 issuewild "digicert.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paragonbank.co.uk
  spf: true
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: paragonbankinggroup.co.uk
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.paragonbank.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 20:05:50 2026 GMT
  host: www.paragonbankinggroup.co.uk
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Paragon Bank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paragon Bank, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Paragon Bank
provider_slug: paragon-bank
slug: paragon-bank-domain-security
source_filename: paragon-bank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paragonbank.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: null\n- host: www.paragonbankinggroup.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 20:05:50 2026 GMT\n  hsts: null\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: paragonbank.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"digicert.com\"\n  - 0 issuewild \"digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: paragonbankinggroup.co.uk\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paragon-bank/refs/heads/main/security/paragon-bank-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Financial Services
- Banking
- Savings
- Mortgages
- Specialist Lender
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Account Information
---
