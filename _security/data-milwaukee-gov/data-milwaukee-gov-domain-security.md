---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "starfieldtech.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "godaddy.com"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: milwaukee.gov
  spf: true
hosts:
- cert_expires: Oct  2 14:31:26 2026 GMT
  host: data.milwaukee.gov
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Data Milwaukee Gov Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Milwaukee Open Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Milwaukee Open Data
provider_slug: data-milwaukee-gov
slug: data-milwaukee-gov-domain-security
source_filename: data-milwaukee-gov-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: data.milwaukee.gov\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:31:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: milwaukee.gov\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"starfieldtech.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/data-milwaukee-gov/refs/heads/main/security/data-milwaukee-gov-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Open Data
- CKAN
- Data Catalog
- DCAT
- Government Data
- Municipal Government
- United States
---
