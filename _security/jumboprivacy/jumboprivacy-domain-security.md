---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: jumboprivacy.com
  spf: true
hosts:
- cert_expires: Sep  2 16:26:49 2026 GMT
  host: www.jumboprivacy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jumboprivacy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jumbo Privacy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Jumbo Privacy
provider_slug: jumboprivacy
slug: jumboprivacy-domain-security
source_filename: jumboprivacy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jumboprivacy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  2 16:26:49 2026 GMT\n  hsts: false\ndomains:\n- domain: jumboprivacy.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jumboprivacy/refs/heads/main/security/jumboprivacy-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Privacy
- Security
- Consumer
- Identity Protection
- Data Protection
- Mobile App
- Defunct
---
