---
api_specs:
- filename: finops-foundation-focus-cost-and-usage-openapi.yml
  format: yaml
  label: FOCUS Cost and Usage API
  slug: focus-cost-and-usage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/openapi/finops-foundation-focus-cost-and-usage-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: finops.org
  spf: true
hosts:
- cert_expires: Oct  3 08:21:44 2026 GMT
  host: www.finops.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 29 00:23:39 2026 GMT
  host: focus.finops.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Finops Foundation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FinOps Foundation, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: FinOps Foundation
provider_slug: finops-foundation
slug: finops-foundation-domain-security
source_filename: finops-foundation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.finops.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 08:21:44 2026 GMT\n  hsts: false\n- host: focus.finops.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 00:23:39 2026 GMT\n  hsts: false\ndomains:\n- domain: finops.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finops-foundation/refs/heads/main/security/finops-foundation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Budgets
- Costs
- FinOps
---
