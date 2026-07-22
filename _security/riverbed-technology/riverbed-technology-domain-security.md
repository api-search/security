---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: riverbed.com
  spf: true
hosts:
- cert_expires: Aug 25 16:46:58 2026 GMT
  host: www.riverbed.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Riverbed Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Riverbed Technology, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Riverbed Technology
provider_slug: riverbed-technology
slug: riverbed-technology-domain-security
source_filename: riverbed-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.riverbed.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 16:46:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: riverbed.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/riverbed-technology/refs/heads/main/security/riverbed-technology-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Enterprise Software
- Observability
- Network Monitoring
- Digital Experience Monitoring
- AIOps
- IT Operations
- Application Performance Monitoring
---
