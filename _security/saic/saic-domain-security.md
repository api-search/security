---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: saic.com
  spf: true
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: www.saic.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Saic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Science Applications International Corporation (SAIC), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Science Applications International Corporation (SAIC)
provider_slug: saic
slug: saic-domain-security
source_filename: saic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.saic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: saic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/saic/refs/heads/main/security/saic-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Defense
- Intelligence
- Federal IT
- Digital Engineering
- Artificial Intelligence
- Cloud
- Cybersecurity
- Mission IT
- Space
- Government Services
- Company
- Fortune 1000
---
