---
api_specs:
- filename: apis.md
  format: yaml
  label: Zocdoc API
  slug: zocdoc-api
  spec_type: OpenAPI
  url: https://api-docs.zocdoc.com/apis.md
description: ''
domains:
- caa:
  - 0 iodef "mailto:action-informationsecurity@zocdoc.com"
  - 0 issue "amazon.com"
  - 0 issue "digicert.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zocdoc.com
  spf: true
hosts:
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: www.zocdoc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 18:53:34 2026 GMT
  host: api-docs.zocdoc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 17 23:59:59 2026 GMT
  host: api-developer.zocdoc.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zocdoc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zocdoc, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zocdoc
provider_slug: zocdoc
slug: zocdoc-domain-security
source_filename: zocdoc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.zocdoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\n- host: api-docs.zocdoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 18:53:34 2026 GMT\n  hsts: false\n- host: api-developer.zocdoc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: zocdoc.com\n  dnssec: false\n  caa:\n  - 0 iodef \"mailto:action-informationsecurity@zocdoc.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"digicert.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zocdoc/refs/heads/main/security/zocdoc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Appointments
- Booking
- Providers
- Insurance
- Telehealth
- Scheduling
---
