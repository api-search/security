---
api_specs:
- filename: hydrata-com-openapi-generated.yml
  format: yaml
  label: Hydrata API
  slug: hydrata-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hydrata-com/openapi/_ae-authored/hydrata-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issuewild ";"
  - 0 iodef "mailto:info@hydrata.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hydrata.com
  spf: true
hosts:
- cert_expires: Dec 25 17:02:41 2026 GMT
  host: hydrata.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Hydrata Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydrata, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hydrata
provider_slug: hydrata-com
slug: hydrata-com-domain-security
source_filename: hydrata-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydrata.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 25 17:02:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hydrata.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \";\"\n  - 0 iodef \"mailto:info@hydrata.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/hydrata-com/security/hydrata-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- hydraulic
- Verification
- Engineering
- Open Source
- Modeling
---
