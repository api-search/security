---
api_specs:
- filename: akamai-api-security-openapi.json
  format: json
  label: Akamai API Security
  slug: api-security
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/openapi/akamai-api-security-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: akamai.com
  spf: true
hosts:
- cert_expires: Dec  2 23:59:59 2026 GMT
  host: www.akamai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 06:16:17 2026 GMT
  host: techdocs.akamai.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akamai Api Security Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akamai API Security, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Akamai API Security
provider_slug: akamai-api-security
slug: akamai-api-security-domain-security
source_filename: akamai-api-security-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akamai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  2 23:59:59 2026 GMT\n  hsts: null\n- host: techdocs.akamai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 06:16:17 2026 GMT\n  hsts: null\ndomains:\n- domain: akamai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akamai-api-security/refs/heads/main/security/akamai-api-security-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- API Discovery
- API Security
- Cloud Security
- Posture Management
- Runtime Protection
- Threat Protection
---
