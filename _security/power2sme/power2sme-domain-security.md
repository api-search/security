---
api_specs:
- filename: power2sme-openapi.json
  format: json
  label: POWER2SME API
  slug: power2sme-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/power2sme/refs/heads/main/openapi/power2sme-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: power2sme.com
  spf: true
hosts:
- cert_expires: Nov 27 23:59:59 2026 GMT
  host: www.power2sme.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Power2Sme Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Power2SME, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Power2SME
provider_slug: power2sme
slug: power2sme-domain-security
source_filename: power2sme-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.power2sme.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: power2sme.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/power2sme/refs/heads/main/security/power2sme-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Marketplaces
- SME
- Procurement
- India
- Onboarding
- OTP
- API
---
