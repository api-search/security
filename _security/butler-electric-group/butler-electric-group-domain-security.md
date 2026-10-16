---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: butler-electric.com
  spf: true
hosts:
- cert_expires: Dec 19 16:17:56 2026 GMT
  host: www.butler-electric.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Butler Electric Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Butler Electric Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Butler Electric Group
provider_slug: butler-electric-group
slug: butler-electric-group-domain-security
source_filename: butler-electric-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.butler-electric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 16:17:56 2026 GMT\n  hsts: false\ndomains:\n- domain: butler-electric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/butler-electric-group/refs/heads/main/security/butler-electric-group-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Electrical
- Contractor
- Residential
- Commercial
---
