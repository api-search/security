---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: sidecarhealth.com
  spf: true
hosts:
- cert_expires: Sep  3 04:32:17 2026 GMT
  host: sidecarhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sidecarhealth Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sidecar Health, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sidecar Health
provider_slug: sidecarhealth
slug: sidecarhealth-domain-security
source_filename: sidecarhealth-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sidecarhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 04:32:17 2026 GMT\n  hsts: false\ndomains:\n- domain: sidecarhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sidecarhealth/refs/heads/main/security/sidecarhealth-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthtech
- Health Insurance
- Insurance
- Healthcare
- Employer Benefits
- Price Transparency
---
