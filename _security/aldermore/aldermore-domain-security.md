---
api_specs:
- filename: aldermore-obie-open-data-openapi.json
  format: json
  label: Aldermore Open Data API (OBIE Standard)
  slug: aldermore-open-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-open-data-openapi.json
- filename: aldermore-obie-account-info-openapi.yaml
  format: yaml
  label: Aldermore Account & Transaction Information API (OBIE Read/Write Standard)
  slug: aldermore-account-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-account-info-openapi.yaml
- filename: aldermore-obie-payment-initiation-openapi.yaml
  format: yaml
  label: Aldermore Payment Initiation API (OBIE Read/Write Standard)
  slug: aldermore-payment-initiation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-payment-initiation-openapi.yaml
- filename: aldermore-obie-confirmation-of-funds-openapi.yaml
  format: yaml
  label: Aldermore Confirmation of Funds API (OBIE Read/Write Standard)
  slug: aldermore-confirmation-of-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/openapi/aldermore-obie-confirmation-of-funds-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aldermore.co.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: openbanking.org.uk
  spf: true
hosts:
- cert_expires: Jan 20 23:59:59 2027 GMT
  host: www.aldermore.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.openbanking.org.uk
  https: false
kind: domain-security
layout: security
method: probed
name: Aldermore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aldermore Bank, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Aldermore Bank
provider_slug: aldermore
slug: aldermore-domain-security
source_filename: aldermore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aldermore.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.openbanking.org.uk\n  https: false\ndomains:\n- domain: aldermore.co.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: openbanking.org.uk\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aldermore/refs/heads/main/security/aldermore-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial Services
- Banking
- Savings
- Specialist Lending
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
---
