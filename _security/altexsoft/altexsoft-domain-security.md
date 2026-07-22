---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: altexsoft.com
  spf: true
hosts:
- cert_expires: Feb 18 23:59:59 2027 GMT
  host: www.altexsoft.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Altexsoft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AltexSoft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: AltexSoft
provider_slug: altexsoft
slug: altexsoft-domain-security
source_filename: altexsoft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.altexsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 18 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: altexsoft.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altexsoft/refs/heads/main/security/altexsoft-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Hospitality
- IT Consulting
- Software Development
- Travel
- Technology Solutions
---
