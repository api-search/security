---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: asocscloud.com
  spf: true
hosts:
- cert_expires: Dec 24 12:07:04 2026 GMT
  host: asocscloud.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Asocs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asocs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Asocs
provider_slug: asocs
slug: asocs-domain-security
source_filename: asocs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asocscloud.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 24 12:07:04 2026 GMT\n  hsts: false\ndomains:\n- domain: asocscloud.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asocs/refs/heads/main/security/asocs-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Industrial 5G
- Private Networks
- AI Positioning
- AI Kits
- Enterprise Solutions
- System Integrators
---
