---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: johnsoncontrols.com
  spf: true
hosts:
- cert_expires: Sep 11 16:37:14 2026 GMT
  host: www.johnsoncontrols.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Johnson Controls Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Johnson Controls, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Johnson Controls
provider_slug: johnson-controls
slug: johnson-controls-domain-security
source_filename: johnson-controls-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.johnsoncontrols.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 16:37:14 2026 GMT\n  hsts: null\ndomains:\n- domain: johnsoncontrols.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johnson-controls/refs/heads/main/security/johnson-controls-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Building Automation
- Energy Storage
- Fire & Security
- HVAC
- Smart Buildings
- Fortune 100
---
