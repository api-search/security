---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: evercontact.com
  spf: true
hosts:
- cert_expires: Aug 29 02:50:03 2026 GMT
  host: www.evercontact.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.evercontact.com
  https: false
kind: domain-security
layout: security
method: probed
name: Evercontact Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Evercontact, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Evercontact
provider_slug: evercontact
slug: evercontact-domain-security
source_filename: evercontact-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.evercontact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 02:50:03 2026 GMT\n  hsts: false\n- host: api.evercontact.com\n  https: false\ndomains:\n- domain: evercontact.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evercontact/refs/heads/main/security/evercontact-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Contact Management
- Contact Data
- Data Enrichment
- Email
- Signature Parsing
- Data Extraction
- CRM
---
