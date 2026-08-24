---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hydrow.com
  spf: true
hosts:
- cert_expires: Oct 23 19:59:10 2026 GMT
  host: hydrow.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hydrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hydrow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hydrow
provider_slug: hydrow
slug: hydrow-domain-security
source_filename: hydrow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hydrow.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 23 19:59:10 2026 GMT\n  hsts: null\ndomains:\n- domain: hydrow.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hydrow/refs/heads/main/security/hydrow-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Connected Fitness
- Consumer Hardware
- Rowing
- Fitness
- Wellness
- Health
- Streaming Media
- Subscription
- Internet of Things
---
