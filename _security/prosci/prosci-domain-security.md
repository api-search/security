---
api_specs:
- filename: prosci-change-management-openapi.yml
  format: yaml
  label: Prosci Change Management
  slug: prosci
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-change-management-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: prosci.com
  spf: true
hosts:
- cert_expires: Aug 25 09:57:58 2026 GMT
  host: www.prosci.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: api.prosci.com
  https: false
kind: domain-security
layout: security
method: probed
name: Prosci Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Prosci, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Prosci
provider_slug: prosci
slug: prosci-domain-security
source_filename: prosci-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.prosci.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:57:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.prosci.com\n  https: false\ndomains:\n- domain: prosci.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/security/prosci-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Change Management
- Methodology
- Training
---
