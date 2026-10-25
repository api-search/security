---
api_specs:
- filename: keysight-technologies-openapi-generated.yml
  format: yaml
  label: Keysight Technologies API
  slug: keysight-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keysight-technologies/refs/heads/main/openapi/_ae-authored/keysight-technologies-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: keysight.com
  spf: true
hosts:
- cert_expires: Nov 28 13:43:17 2026 GMT
  host: www.keysight.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Keysight Technologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Keysight Technologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Keysight Technologies
provider_slug: keysight-technologies
slug: keysight-technologies-domain-security
source_filename: keysight-technologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.keysight.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 13:43:17 2026 GMT\n  hsts: null\ndomains:\n- domain: keysight.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keysight-technologies/refs/heads/main/security/keysight-technologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Network Testing
- Test and Measurement
- Performance Testing
- Security Testing
- Electronics
- Traffic Generation
- MCP
---
