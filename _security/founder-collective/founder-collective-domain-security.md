---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: foundercollective.com
  spf: true
hosts:
- cert_expires: Sep 11 06:32:01 2026 GMT
  host: www.foundercollective.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Founder Collective Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Founder Collective, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Founder Collective
provider_slug: founder-collective
slug: founder-collective-domain-security
source_filename: founder-collective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foundercollective.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 06:32:01 2026 GMT\n  hsts: false\ndomains:\n- domain: foundercollective.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/founder-collective/refs/heads/main/security/founder-collective-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Venture Capital
- Seed Stage
- Pre-Seed
- Startups
- Investment
- Sector Agnostic
---
