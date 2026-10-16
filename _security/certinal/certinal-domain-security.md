---
api_specs:
- filename: certinal-openapi-generated.yml
  format: yaml
  label: Certinal API
  slug: certinal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/certinal/refs/heads/main/openapi/_ae-authored/certinal-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: certinal.com
  spf: true
hosts:
- cert_expires: Nov 20 09:23:42 2026 GMT
  host: certinal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Certinal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Certinal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Certinal
provider_slug: certinal
slug: certinal-domain-security
source_filename: certinal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: certinal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 20 09:23:42 2026 GMT\n  hsts: false\ndomains:\n- domain: certinal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/certinal/refs/heads/main/security/certinal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Healthcare
- Consent
- Compliance
- eSignature
- EHR Integration
- Regulatory
---
