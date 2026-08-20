---
description: ''
domains:
- caa:
  - 0 issuewild "entrust.com"
  - 0 issuewild "godaddy.com"
  - 0 issue "digicert.com"
  - 0 issue "godaddy.com"
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: servus.ca
  spf: true
hosts:
- cert_expires: Oct 27 23:59:59 2026 GMT
  host: www.servus.ca
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Servus Credit Union Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Servus Credit Union, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Servus Credit Union
provider_slug: servus-credit-union
slug: servus-credit-union-domain-security
source_filename: servus-credit-union-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.servus.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 27 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: servus.ca\n  dnssec: true\n  caa:\n  - 0 issuewild \"entrust.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/servus-credit-union/refs/heads/main/security/servus-credit-union-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Financial-Services
- Banking
- Canada
- Credit Union
- Cooperative
- Alberta
- Open Banking
- Data Aggregation
---
