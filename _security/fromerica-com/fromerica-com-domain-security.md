---
api_specs:
- filename: fromerica-com-openapi-generated.yml
  format: yaml
  label: Fromerica API
  slug: fromerica-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fromerica-com/openapi/_ae-authored/fromerica-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 iodef "mailto:info@fromerica.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fromerica.com
  spf: true
hosts:
- cert_expires: Mar  9 07:01:56 2027 GMT
  host: fromerica.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Fromerica Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fromerica, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Fromerica
provider_slug: fromerica-com
slug: fromerica-com-domain-security
source_filename: fromerica-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fromerica.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  9 07:01:56 2027 GMT\n  hsts: null\ndomains:\n- domain: fromerica.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:info@fromerica.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/fromerica-com/security/fromerica-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Marketplace
- B2B
- Manufacturing
- Export
- Import
---
