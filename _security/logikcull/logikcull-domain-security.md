---
api_specs:
- filename: logikcull
  format: yaml
  label: Logikcull API
  slug: logikcull-api
  spec_type: OpenAPI
  url: https://docs.revealdata.com/logikcull
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: logikcull.com
  spf: true
hosts:
- cert_expires: Aug 15 12:59:07 2026 GMT
  host: www.logikcull.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 23:59:59 2026 GMT
  host: api.logikcull.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Logikcull Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Logikcull, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Logikcull
provider_slug: logikcull
slug: logikcull-domain-security
source_filename: logikcull-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.logikcull.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 15 12:59:07 2026 GMT\n  hsts: false\n- host: api.logikcull.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: logikcull.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/logikcull/refs/heads/main/security/logikcull-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- eDiscovery
- Legal
- Document Management
- Legal Holds
- Redaction
- Production Sets
- Cloud
---
