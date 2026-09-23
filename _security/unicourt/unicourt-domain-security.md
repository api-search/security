---
api_specs:
- filename: unicourt-openapi-generated.yml
  format: yaml
  label: UniCourt API
  slug: unicourt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unicourt/refs/heads/main/openapi/_ae-authored/unicourt-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:itadmin@unicourt.com"
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: unicourt.com
  spf: true
hosts:
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: unicourt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: docs.unicourt.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Unicourt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UniCourt, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: UniCourt
provider_slug: unicourt
slug: unicourt-domain-security
source_filename: unicourt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: unicourt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.unicourt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: unicourt.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:itadmin@unicourt.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unicourt/refs/heads/main/security/unicourt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Legal Tech
- Data Analytics
- Litigation
- Platform
---
