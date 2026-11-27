---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: cordering.com
  spf: true
hosts:
- cert_expires: Jan 27 19:20:09 2027 GMT
  host: cordering.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: COrdering Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for COrdering, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: COrdering
provider_slug: cordering-com
slug: cordering-com-domain-security
source_filename: cordering-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cordering.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 19:20:09 2027 GMT\n  hsts: false\ndomains:\n- domain: cordering.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/cordering-com/security/cordering-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Food Ordering
- Restaurant
- Catering
- Corporate Meals
- Food Delivery
- Mobile App
- MCP
- Serbia
---
