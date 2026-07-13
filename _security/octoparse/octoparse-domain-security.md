---
api_specs:
- filename: octoparse-openapi.yml
  format: yaml
  label: Octoparse
  slug: octoparse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/openapi/octoparse-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: octoparse.com
  spf: true
hosts:
- cert_expires: Aug 13 23:59:59 2026 GMT
  host: www.octoparse.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 10 18:33:54 2026 GMT
  host: openapi.octoparse.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Octoparse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Octoparse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Octoparse
provider_slug: octoparse
slug: octoparse-domain-security
source_filename: octoparse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.octoparse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 13 23:59:59 2026 GMT\n  hsts: false\n- host: openapi.octoparse.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 18:33:54 2026 GMT\n  hsts: null\ndomains:\n- domain: octoparse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/octoparse/refs/heads/main/security/octoparse-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Harvesting
- Scraping
---
