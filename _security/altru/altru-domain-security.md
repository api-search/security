---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:domains@icims.com"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: altrulabs.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: altrulabs.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Altru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Altru, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Altru
provider_slug: altru
slug: altru-domain-security
source_filename: altru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: altrulabs.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: altrulabs.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:domains@icims.com\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/altru/refs/heads/main/security/altru-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Company
- Talent Acquisition
- Recruitment Marketing
- HR Tech
- Video
- Employee Generated Content
- Employer Branding
- Acquired
---
