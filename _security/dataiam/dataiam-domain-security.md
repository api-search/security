---
description: ''
domains:
- caa:
  - 0 issuewild "comodoca.com"
  - 0 issue "amazon.com"
  - 0 issue "awstrust.com"
  - 0 issue "digicert.com"
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: dataiam.com
  spf: true
hosts:
- cert_expires: Feb 19 23:59:59 2027 GMT
  host: dataiam.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Dataiam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Data I Am, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Data I Am
provider_slug: dataiam
slug: dataiam-domain-security
source_filename: dataiam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dataiam.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: dataiam.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"comodoca.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/dataiam/security/dataiam-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Salesforce
- Data Integration
- Financial Services
---
