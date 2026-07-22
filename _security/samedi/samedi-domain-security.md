---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "amazonaws.com"
  - 0 iodef "mailto:devops@samedi.de"
  - 0 issue "ssl.com"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: samedi.de
  spf: true
hosts:
- cert_expires: Aug 29 06:39:42 2026 GMT
  host: www.samedi.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Samedi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for samedi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: samedi
provider_slug: samedi
slug: samedi-domain-security
source_filename: samedi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.samedi.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 06:39:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: samedi.de\n  dnssec: true\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazonaws.com\"\n  - 0 iodef \"mailto:devops@samedi.de\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/samedi/refs/heads/main/security/samedi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Healthcare
- Scheduling
- Appointments
- Booking
- Patient Engagement
- OAuth
- FHIR
- Telemedicine
- Germany
---
