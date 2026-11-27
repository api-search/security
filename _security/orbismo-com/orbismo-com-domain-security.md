---
api_specs:
- filename: orbismo-com-openapi-generated.yml
  format: yaml
  label: Orbismo API
  slug: orbismo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/orbismo-com/openapi/_ae-authored/orbismo-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 iodef "mailto:infra@ghzlab.com"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: orbismo.com
  spf: true
hosts:
- cert_expires: Dec 24 00:38:20 2026 GMT
  host: orbismo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Orbismo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbismo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Orbismo
provider_slug: orbismo-com
slug: orbismo-com-domain-security
source_filename: orbismo-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbismo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 00:38:20 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orbismo.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 iodef \"mailto:infra@ghzlab.com\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/orbismo-com/security/orbismo-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- Worldbuilding
- Creative
- Collaboration
- Software-as-a-Service
---
