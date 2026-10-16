---
api_specs:
- filename: laserfiche-api-openapi-generated.yml
  format: yaml
  label: Laserfiche api API
  slug: api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/_ae-authored/laserfiche-api-openapi-generated.yml
- filename: laserfiche-core-openapi-generated.yml
  format: yaml
  label: Laserfiche core API
  slug: core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/_ae-authored/laserfiche-core-openapi-generated.yml
- filename: laserfiche-guides-openapi-generated.yml
  format: yaml
  label: Laserfiche Guides API
  slug: guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/openapi/_ae-authored/laserfiche-guides-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "amazon.com"
  - 0 issuewild "godaddy.com"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: laserfiche.com
  spf: true
hosts:
- cert_expires: Dec 30 06:15:35 2026 GMT
  host: www.laserfiche.com
  hsts: true
  hsts_max_age: 31622400
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Laserfiche Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Laserfiche, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Laserfiche
provider_slug: laserfiche
slug: laserfiche-domain-security
source_filename: laserfiche-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.laserfiche.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 06:15:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31622400\ndomains:\n- domain: laserfiche.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"amazon.com\"\n  - 0 issuewild \"godaddy.com\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/laserfiche/refs/heads/main/security/laserfiche-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- EnterpriseContentManagement
- DocumentManagement
- ProcessAutomation
- AI
---
