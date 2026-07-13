---
api_specs:
- filename: lens-openapi.yml
  format: yaml
  label: Lens API
  slug: lens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lens/refs/heads/main/openapi/lens-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lens.org
  spf: true
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: www.lens.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 28 17:07:51 2026 GMT
  host: docs.api.lens.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 23:59:59 2026 GMT
  host: api.lens.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lens Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lens, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lens
provider_slug: lens
slug: lens-domain-security
source_filename: lens-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lens.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.api.lens.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:07:51 2026 GMT\n  hsts: false\n- host: api.lens.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lens.org\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lens/refs/heads/main/security/lens-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Scholarly
- Patents
- Research
- Science
- Open Data
---
