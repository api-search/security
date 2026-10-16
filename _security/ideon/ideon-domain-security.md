---
api_specs:
- filename: ideon-openapi-generated.yml
  format: yaml
  label: Ideon API
  slug: ideon-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ideon/refs/heads/main/openapi/_ae-authored/ideon-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ideonapi.com
  spf: true
hosts:
- cert_expires: Nov 29 13:46:25 2026 GMT
  host: www.ideonapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ideon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ideon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ideon
provider_slug: ideon
slug: ideon-domain-security
source_filename: ideon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ideonapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 13:46:25 2026 GMT\n  hsts: false\ndomains:\n- domain: ideonapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ideon/refs/heads/main/security/ideon-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Benefits
- Data
- APIs
- HealthTech
---
