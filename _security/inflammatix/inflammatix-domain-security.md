---
api_specs:
- filename: inflammatix-content-openapi.yml
  format: yaml
  label: Inflammatix Site Content API
  slug: site-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-content-openapi.yml
- filename: inflammatix-support-content-openapi.yml
  format: yaml
  label: Inflammatix Support and Training Content API
  slug: support-content
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/openapi/inflammatix-support-content-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: inflammatix.com
  spf: true
hosts:
- cert_expires: Sep  9 12:19:51 2026 GMT
  host: inflammatix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 20:32:35 2026 GMT
  host: support.inflammatix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Inflammatix Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inflammatix, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Inflammatix
provider_slug: inflammatix
slug: inflammatix-domain-security
source_filename: inflammatix-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inflammatix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 12:19:51 2026 GMT\n  hsts: false\n- host: support.inflammatix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 20:32:35 2026 GMT\n  hsts: false\ndomains:\n- domain: inflammatix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inflammatix/refs/heads/main/security/inflammatix-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Health
- Healthcare
- Diagnostics
- Medical Devices
- In Vitro Diagnostics
- Molecular Diagnostics
- Sepsis
- Machine Learning
- Life Sciences
- Point of Care
- Content
---
