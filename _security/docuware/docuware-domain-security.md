---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: docuware.com
  spf: true
hosts:
- cert_expires: Nov 27 23:51:47 2026 GMT
  host: start.docuware.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Docuware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DocuWare, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DocuWare
provider_slug: docuware
slug: docuware-domain-security
source_filename: docuware-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: start.docuware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:51:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: docuware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docuware/refs/heads/main/security/docuware-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Document Management
- Workflow Automation
- Intelligent Document Processing
- Cloud
- Enterprise Content Management
- Invoice Processing
- Secure Archiving
---
