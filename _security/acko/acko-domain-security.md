---
api_specs:
- filename: acko-apisetu-openapi-original.json
  format: json
  label: Acko General Insurance (API Setu / DigiLocker)
  slug: acko-general-insurance-api-setu-digilocker
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acko/refs/heads/main/openapi/acko-apisetu-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: acko.com
  spf: true
hosts:
- cert_expires: Aug 18 13:46:33 2026 GMT
  host: www.acko.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acko Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acko, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Acko
provider_slug: acko
slug: acko-domain-security
source_filename: acko-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acko.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 18 13:46:33 2026 GMT\n  hsts: true\n  hsts_max_age: 0\ndomains:\n- domain: acko.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acko/refs/heads/main/security/acko-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Consumer
- Insurance
- InsurTech
- Financial Services
- Digital Insurance
- India
- Embedded Insurance
---
