---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aceiss.com
  spf: true
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: www.aceiss.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aceiss Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aceiss, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Aceiss
provider_slug: aceiss
slug: aceiss-domain-security
source_filename: aceiss-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aceiss.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: aceiss.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aceiss/refs/heads/main/security/aceiss-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Security
- Identity and Access Management
- Access Control
- Governance
- Compliance
- Monitoring
- GitHub
- Insider Threat
- Zero Trust
---
