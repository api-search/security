---
api_specs:
- filename: loopme-reporting-openapi.yml
  format: yaml
  label: LoopMe Reporting API
  slug: loopme-reporting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopme/refs/heads/main/openapi/loopme-reporting-openapi.yml
- filename: loopme-s2s-openapi.yml
  format: yaml
  label: LoopMe S2S Ad Request API
  slug: loopme-s2s-ad-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loopme/refs/heads/main/openapi/loopme-s2s-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:devops@loopme.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loopme.com
  spf: true
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "digicert.com"
  - 0 iodef "mailto:devops@loopme.com"
  - 0 issue "sectigo.com"
  dmarc: false
  dnssec: false
  domain: loopme.me
  spf: true
hosts:
- cert_expires: Sep 16 09:22:00 2026 GMT
  host: reports.loopme.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 16 09:22:00 2026 GMT
  host: loopme.me
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Loopme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LoopMe, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: LoopMe
provider_slug: loopme
slug: loopme-domain-security
source_filename: loopme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: reports.loopme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 09:22:00 2026 GMT\n  hsts: null\n- host: loopme.me\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 09:22:00 2026 GMT\n  hsts: false\ndomains:\n- domain: loopme.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:devops@loopme.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: loopme.me\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"digicert.com\"\n  - 0 iodef \"mailto:devops@loopme.com\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loopme/refs/heads/main/security/loopme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Advertising
- AdTech
- Mobile Advertising
- CTV
- Reporting
- Programmatic
- Ai Enterprise Software
- SDK
---
