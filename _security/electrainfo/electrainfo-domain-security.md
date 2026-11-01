---
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issuewild "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild "Digicert.com"
  - 0 issue "Digicert.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: electrainfo.com
  spf: true
hosts:
- cert_expires: Dec 29 23:59:59 2026 GMT
  host: electrainfo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Electrainfo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gresham Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Gresham Technologies
provider_slug: electrainfo
slug: electrainfo-domain-security
source_filename: electrainfo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: electrainfo.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: electrainfo.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"Digicert.com\"\n  - 0 issue \"Digicert.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/electrainfo/security/electrainfo-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Enterprise Data Management
- Reconciliation
- Regulatory Reporting
- Data Services
- Financial Services
- ESG Data
- Trading Data
---
