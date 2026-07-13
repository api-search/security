---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dfsco.com
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: www.dfsco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: developer.dfsco.com
  https: false
- host: api.dfsco.com
  https: false
kind: domain-security
layout: security
method: probed
name: Donnelley Financial Solutions Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Donnelley Financial Solutions, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Donnelley Financial Solutions
provider_slug: donnelley-financial-solutions
slug: donnelley-financial-solutions-domain-security
source_filename: donnelley-financial-solutions-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dfsco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.dfsco.com\n  https: false\n- host: api.dfsco.com\n  https: false\ndomains:\n- domain: dfsco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/donnelley-financial-solutions/refs/heads/main/security/donnelley-financial-solutions-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Financial
- Regulatory Compliance
- Software
---
