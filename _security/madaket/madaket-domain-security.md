---
api_specs:
- filename: madaket-provider-api.yml
  format: yaml
  label: Madaket Provider API
  slug: provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madaket/refs/heads/main/openapi/madaket-provider-api.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: madakethealth.com
  spf: true
hosts:
- cert_expires: Oct 18 17:24:36 2026 GMT
  host: www.madakethealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: provider.madakethealth.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Madaket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Madaket, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Madaket
provider_slug: madaket
slug: madaket-domain-security
source_filename: madaket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.madakethealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 17:24:36 2026 GMT\n  hsts: false\n- host: provider.madakethealth.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: madakethealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madaket/refs/heads/main/security/madaket-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthcare
- Provider Data Management
- Payer Enrollment
- Credentialing
- Provider Directory
- EDI
- Health Insurance
- Licensing
- Healthcare Administration
---
