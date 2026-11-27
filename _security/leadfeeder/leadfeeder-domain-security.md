---
api_specs:
- filename: leadfeeder-openapi-generated.yml
  format: yaml
  label: Leadfeeder API
  slug: leadfeeder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfeeder/openapi/_ae-authored/leadfeeder-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: leadfeeder.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: leadfeeder.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Leadfeeder Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Leadfeeder, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Leadfeeder
provider_slug: leadfeeder
slug: leadfeeder-domain-security
source_filename: leadfeeder-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: leadfeeder.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: leadfeeder.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/leadfeeder/security/leadfeeder-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- B2B
- Analytics
- Lead Generation
- Marketing
---
