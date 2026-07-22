---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "certainly.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codementor.io
  spf: true
hosts:
- cert_expires: Oct  7 00:11:22 2026 GMT
  host: codementor.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codementor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CodeMentor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: CodeMentor
provider_slug: codementor
slug: codementor-domain-security
source_filename: codementor-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codementor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 00:11:22 2026 GMT\n  hsts: null\ndomains:\n- domain: codementor.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"certainly.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codementor/refs/heads/main/security/codementor-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Developer Mentorship
- Freelance Marketplace
- Software Development
- Hiring
- Learning
- Community
---
