---
api_specs:
- filename: kviria-com-account-api-openapi.yml
  format: yaml
  label: Kviria Account API
  slug: kviria-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-account-api-openapi.yml
- filename: kviria-com-agent-api-openapi.yml
  format: yaml
  label: Kviria Agent API
  slug: kviria-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-agent-api-openapi.yml
- filename: kviria-com-healthz-api-openapi.yml
  format: yaml
  label: Kviria Healthz API
  slug: kviria-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-healthz-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: kviria.com
  spf: true
hosts:
- cert_expires: Jan 20 12:11:40 2027 GMT
  host: kviria.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kviria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kviria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Kviria
provider_slug: kviria-com
slug: kviria-com-domain-security
source_filename: kviria-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kviria.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 20 12:11:40 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: kviria.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/kviria-com/security/kviria-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- location understanding
- AI Agents
- Privacy
---
