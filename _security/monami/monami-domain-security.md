---
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 iodef "mailto:admin@monami.io"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: monami.io
  spf: true
hosts:
- cert_expires: Dec 22 23:59:59 2026 GMT
  host: monami.io
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Monami Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mon Ami, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Mon Ami
provider_slug: monami
slug: monami-domain-security
source_filename: monami-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: monami.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 22 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: monami.io\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 iodef \"mailto:admin@monami.io\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monami/refs/heads/main/security/monami-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Aging Services
- Disability Services
- Case Management
- Healthcare
- Government
- Medicaid
- HCBS
- Ombudsman
- FHIR
---
