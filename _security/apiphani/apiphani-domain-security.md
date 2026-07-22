---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: apiphani.io
  spf: true
hosts:
- cert_expires: Sep  7 11:10:59 2026 GMT
  host: www.apiphani.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Apiphani Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apiphani, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Apiphani
provider_slug: apiphani
slug: apiphani-domain-security
source_filename: apiphani-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.apiphani.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:10:59 2026 GMT\n  hsts: false\ndomains:\n- domain: apiphani.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiphani/refs/heads/main/security/apiphani-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Managed Services
- SAP
- Application Management
- Cloud
- Observability
- AIOps
- Enterprise Software
- Security
---
