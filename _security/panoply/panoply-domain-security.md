---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issuewild "godaddy.com"
  - 0 iodef "mailto:yonil@sqreamtech.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: panoply.io
  spf: true
hosts:
- cert_expires: Nov 30 11:43:38 2026 GMT
  host: panoply.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Panoply Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Panoply, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Panoply
provider_slug: panoply
slug: panoply-domain-security
source_filename: panoply-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: panoply.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 30 11:43:38 2026 GMT\n  hsts: false\ndomains:\n- domain: panoply.io\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 iodef \"mailto:yonil@sqreamtech.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/panoply/refs/heads/main/security/panoply-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Data Warehouse
- ELT
- Data Integration
- Analytics
- Cloud Data Platform
- Connectors
---
