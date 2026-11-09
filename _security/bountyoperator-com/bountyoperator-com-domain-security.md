---
api_specs:
- filename: bountyoperator-com-openapi-generated.yml
  format: yaml
  label: Bounty Operator API
  slug: bountyoperator-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bountyoperator-com/openapi/_ae-authored/bountyoperator-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bountyoperator.com
  spf: true
hosts:
- cert_expires: Dec 31 07:54:35 2026 GMT
  host: bountyoperator.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bountyoperator Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bounty Operator, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bounty Operator
provider_slug: bountyoperator-com
slug: bountyoperator-com-domain-security
source_filename: bountyoperator-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bountyoperator.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 07:54:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bountyoperator.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/bountyoperator-com/security/bountyoperator-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Security
- Bug Bounty
- Review
- Artificial Intelligence
---
