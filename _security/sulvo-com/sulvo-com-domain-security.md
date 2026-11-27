---
api_specs:
- filename: sulvo-com-openapi-generated.yml
  format: yaml
  label: Sulvo API
  slug: sulvo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sulvo-com/openapi/_ae-authored/sulvo-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: true
  domain: sulvo.com
  spf: true
hosts:
- cert_expires: Feb 19 23:25:03 2027 GMT
  host: sulvo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Sulvo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sulvo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Sulvo
provider_slug: sulvo-com
slug: sulvo-com-domain-security
source_filename: sulvo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sulvo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 19 23:25:03 2027 GMT\n  hsts: false\ndomains:\n- domain: sulvo.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/sulvo-com/security/sulvo-com-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Advertising
- Revenue
- Analytics
- Publishers
---
