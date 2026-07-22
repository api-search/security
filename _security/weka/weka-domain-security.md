---
api_specs:
- filename: weka-openapi-original.json
  format: json
  label: WEKA REST API
  slug: weka-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weka/refs/heads/main/openapi/weka-openapi-original.json
description: ''
domains:
- caa:
  - 0 iodef "mailto:certs@weka.io"
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "amazon.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: weka.io
  spf: true
hosts:
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: weka.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weka Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Weka, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Weka
provider_slug: weka
slug: weka-domain-security
source_filename: weka-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weka.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: weka.io\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:certs@weka.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weka/refs/heads/main/security/weka-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI Storage
- Data Platform
- High Performance Computing
- File System
- Object Storage
- Kubernetes
- Cloud Infrastructure
---
