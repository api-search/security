---
api_specs:
- filename: cloudleaf-token-api-openapi.yml
  format: yaml
  label: ParkourSC Token API
  slug: cloudleaf-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudleaf/refs/heads/main/openapi/cloudleaf-token-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: parkoursc.com
  spf: true
hosts:
- cert_expires: Nov  9 15:27:05 2026 GMT
  host: www.parkoursc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cloudleaf Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParkourSC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ParkourSC
provider_slug: cloudleaf
slug: cloudleaf-domain-security
source_filename: cloudleaf-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.parkoursc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 15:27:05 2026 GMT\n  hsts: false\ndomains:\n- domain: parkoursc.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudleaf/refs/heads/main/security/cloudleaf-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Supply Chain
- Artificial Intelligence
- DigitalTwin
- DecisionIntelligence
- Logistics
- Cloud
---
