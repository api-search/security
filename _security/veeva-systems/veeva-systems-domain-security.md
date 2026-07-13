---
api_specs:
- filename: veeva-systems-openapi.yml
  format: yaml
  label: Veeva Systems API
  slug: veeva-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veeva-systems/refs/heads/main/openapi/veeva-systems-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  - 0 issue "starfieldtech.com"
  - 0 issuewild "amazon.com"
  - 0 issuewild "amazonaws.com"
  - 0 issuewild "amazontrust.com"
  - 0 issuewild "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: veeva.com
  spf: true
hosts:
- cert_expires: Aug 27 15:10:08 2026 GMT
  host: www.veeva.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  6 23:59:59 2027 GMT
  host: developer.veeva.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: api.veeva.com
  https: false
kind: domain-security
layout: security
method: probed
name: Veeva Systems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Veeva Systems, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Veeva Systems
provider_slug: veeva-systems
slug: veeva-systems-domain-security
source_filename: veeva-systems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.veeva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 27 15:10:08 2026 GMT\n  hsts: true\n  hsts_max_age: 300\n- host: developer.veeva.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 23:59:59 2027 GMT\n  hsts: false\n- host: api.veeva.com\n  https: false\ndomains:\n- domain: veeva.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"amazonaws.com\"\n  - 0 issuewild \"amazontrust.com\"\n  - 0 issuewild \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veeva-systems/refs/heads/main/security/veeva-systems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Healthcare
- SaaS
- Life Sciences
---
