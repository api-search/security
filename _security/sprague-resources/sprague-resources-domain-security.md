---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: spragueenergy.com
  spf: true
hosts:
- cert_expires: Jul 20 18:21:09 2026 GMT
  host: www.spragueenergy.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sprague Resources Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sprague Resources, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Sprague Resources
provider_slug: sprague-resources
slug: sprague-resources-domain-security
source_filename: sprague-resources-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.spragueenergy.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jul 20 18:21:09 2026 GMT\n  hsts: false\ndomains:\n- domain: spragueenergy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprague-resources/refs/heads/main/security/sprague-resources-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Energy
- Petroleum
- Natural Gas
- Fuel Distribution
- Materials Handling
- Northeast
---
