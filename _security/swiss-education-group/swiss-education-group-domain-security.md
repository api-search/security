---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: swisseducation.com
  spf: true
hosts:
- cert_expires: Sep  6 15:33:52 2026 GMT
  host: www.swisseducation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Swiss Education Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Swiss Education Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Swiss Education Group
provider_slug: swiss-education-group
slug: swiss-education-group-domain-security
source_filename: swiss-education-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.swisseducation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 15:33:52 2026 GMT\n  hsts: false\ndomains:\n- domain: swisseducation.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiss-education-group/refs/heads/main/security/swiss-education-group-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Education
- Hospitality
- Hotel Management
- Culinary Arts
- Switzerland
---
