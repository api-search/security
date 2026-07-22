---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rainwalkpetinsurance.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: rainwalk.io
  spf: true
hosts:
- cert_expires: Oct  8 21:02:53 2026 GMT
  host: rainwalkpetinsurance.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: api.rainwalk.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rainwalk Technology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rainwalk Technology, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Rainwalk Technology
provider_slug: rainwalk-technology
slug: rainwalk-technology-domain-security
source_filename: rainwalk-technology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: rainwalkpetinsurance.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 21:02:53 2026 GMT\n  hsts: false\n- host: api.rainwalk.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: rainwalkpetinsurance.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: rainwalk.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainwalk-technology/refs/heads/main/security/rainwalk-technology-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Insurance
- Pet Insurance
- Embedded Insurance
- Insurtech
- White Label
- Partner API
---
