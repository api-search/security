---
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "godaddy.com"
  - 0 issue "starfieldtech.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: censia.com
  spf: true
hosts:
- cert_expires: Dec 29 20:29:22 2026 GMT
  host: www.censia.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Censia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Censia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Censia
provider_slug: censia
slug: censia-domain-security
source_filename: censia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.censia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 20:29:22 2026 GMT\n  hsts: false\ndomains:\n- domain: censia.com\n  dnssec: false\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"godaddy.com\"\n  - 0 issue \"starfieldtech.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/censia/refs/heads/main/security/censia-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Artificial Intelligence
- Workforce Intelligence
- Talent Analytics
- Talent Mobility
- Upskilling
- Enterprise
---
