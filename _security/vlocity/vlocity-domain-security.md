---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_delegated_to: _dmarc.reject100.salesforce.com
  dmarc_policy: reject
  dnssec: true
  domain: vlocity.com
  spf: true
  spf_includes:
  - _spf.google.com
  - _spf.salesforce.com
  - aspmx.pardot.com
hosts:
- host: www.vlocity.com
  hsts: true
  hsts_max_age: 31536000
  http_status: 503
  https: true
  tls_cert_not_after: '2026-12-17'
  tls_cert_org: Salesforce, Inc.
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vlocity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vlocity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Vlocity
provider_slug: vlocity
slug: vlocity-domain-security
source_filename: vlocity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: dig + openssl + curl HEAD against vlocity.com\nnote: >-\n  Vlocity was acquired by Salesforce in 2020 and folded into Salesforce\n  Industries / OmniStudio; vlocity.com is no longer an independent developer\n  surface. The probe confirms Salesforce now operates the domain: SPF includes\n  _spf.salesforce.com, DMARC is delegated to _dmarc.reject100.salesforce.com,\n  and the TLS certificate is issued to O=Salesforce, Inc. The site itself\n  returns HTTP 503 (Akamai) at the application layer.\nhosts:\n  - host: www.vlocity.com\n    https: true\n    http_status: 503\n    tls_version: TLSv1.3\n    tls_cert_org: Salesforce, Inc.\n    tls_cert_not_after: '2026-12-17'\n    hsts: true\n    hsts_max_age: 31536000\ndomains:\n  - domain: vlocity.com\n    dnssec: true\n    caa: []\n    spf: true\n    spf_includes:\n      - _spf.google.com\n      - _spf.salesforce.com\n      - aspmx.pardot.com\n    dmarc: true\n    dmarc_policy: reject\n\
  \    dmarc_delegated_to: _dmarc.reject100.salesforce.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vlocity/refs/heads/main/security/vlocity-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cloud
- CRM
- Industry Cloud
- Low-Code
- Salesforce
- Acquired
---
