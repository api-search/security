---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: docufree.com
  spf: true
hosts:
- cert_expires: Aug 13 16:25:50 2026 GMT
  host: www.docufree.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Image Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Image API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Image API
provider_slug: image-api
slug: image-api-domain-security
source_filename: image-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.docufree.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 16:25:50 2026 GMT\n  hsts: false\ndomains:\n- domain: docufree.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/image-api/refs/heads/main/security/image-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Business Process Automation
- Digital Mailroom
- Digitization
- Document Management
- Electronic Signature
- Forms
---
