---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: civicroundtable.com
  spf: true
hosts:
- cert_expires: Sep 30 05:11:00 2026 GMT
  host: www.civicroundtable.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civic Roundtable Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civic Roundtable, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Civic Roundtable
provider_slug: civic-roundtable
slug: civic-roundtable-domain-security
source_filename: civic-roundtable-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.civicroundtable.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:11:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: civicroundtable.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civic-roundtable/refs/heads/main/security/civic-roundtable-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- GovTech
- Public Sector
- Government Operations
- Collaboration
- Knowledge Management
- CRM
- Civic
---
