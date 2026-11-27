---
api_specs:
- filename: temporevenue-com-credits-api-openapi.yml
  format: yaml
  label: TempoRevenue Credits API
  slug: temporevenue-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temporevenue-com/openapi/temporevenue-com-credits-api-openapi.yml
- filename: temporevenue-com-proposals-api-openapi.yml
  format: yaml
  label: TempoRevenue Proposals API
  slug: temporevenue-com-proposals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/temporevenue-com/openapi/temporevenue-com-proposals-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dns_aid:
    checked: '2026-11-26'
    published: false
  dnssec: false
  domain: temporevenue.com
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: temporevenue.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: TempoRevenue Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TempoRevenue, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TempoRevenue
provider_slug: temporevenue-com
slug: temporevenue-com-domain-security
source_filename: temporevenue-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: temporevenue.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: temporevenue.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n  dns_aid:\n    checked: '2026-11-26'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/temporevenue-com/security/temporevenue-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- AI
- Contract
- Automation
- Freelance
- SmallBusiness
---
