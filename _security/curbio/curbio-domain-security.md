---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: curbio.com
  spf: true
hosts:
- cert_expires: Dec 18 05:16:06 2026 GMT
  host: curbio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Curbio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Curbio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Curbio
provider_slug: curbio
slug: curbio-domain-security
source_filename: curbio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: curbio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 05:16:06 2026 GMT\n  hsts: false\ndomains:\n- domain: curbio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/curbio/refs/heads/main/security/curbio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Home Renovation
- Real Estate
- Remodeling
- On-Market Concierge
- USA
---
