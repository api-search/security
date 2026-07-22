---
api_specs:
- filename: remote-openapi-original.json
  format: json
  label: Remote API
  slug: remote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/remote/refs/heads/main/openapi/remote-openapi-original.json
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:sre-team@remote.com"
  - 0 issue "amazontrust.com"
  - 0 issue "godaddy.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: remote.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: remote-sandbox.com
  spf: true
hosts:
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: gateway.remote.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 23:59:59 2026 GMT
  host: gateway.remote-sandbox.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Remote Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Remote, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Remote
provider_slug: remote
slug: remote-domain-security
source_filename: remote-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gateway.remote.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\n- host: gateway.remote-sandbox.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: remote.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:sre-team@remote.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: remote-sandbox.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/remote/refs/heads/main/security/remote-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- HR
- Payroll
- Employer of Record
- Global Employment
- Contractors
- Benefits
- Compliance
- Human Resources
---
