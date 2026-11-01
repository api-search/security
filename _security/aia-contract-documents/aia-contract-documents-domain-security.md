---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aiacontracts.com
  spf: true
hosts:
- cert_expires: Mar 18 17:04:50 2027 GMT
  host: aiacontracts.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aia Contract Documents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AIA Contract Documents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: AIA Contract Documents
provider_slug: aia-contract-documents
slug: aia-contract-documents-domain-security
source_filename: aia-contract-documents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aiacontracts.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 17:04:50 2027 GMT\n  hsts: false\ndomains:\n- domain: aiacontracts.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/aia-contract-documents/security/aia-contract-documents-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Construction
- Contracts
- Architecture
- Software
---
