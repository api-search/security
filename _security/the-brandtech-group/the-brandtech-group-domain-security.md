---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: thebrandtechgroup.com
  spf: true
hosts:
- cert_expires: Nov 13 23:08:10 2026 GMT
  host: thebrandtechgroup.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: The Brandtech Group Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Brandtech Group, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: The Brandtech Group
provider_slug: the-brandtech-group
slug: the-brandtech-group-domain-security
source_filename: the-brandtech-group-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thebrandtechgroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 13 23:08:10 2026 GMT\n  hsts: false\ndomains:\n- domain: thebrandtechgroup.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-brandtech-group/refs/heads/main/security/the-brandtech-group-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Marketing
- Advertising
- Generative AI
- Creative
- Marketing Technology
- Retail Media
- Analytics
- Agency
---
