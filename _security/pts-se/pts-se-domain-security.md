---
description: ''
domains:
- caa:
  - 0 iodef "mailto:postmaster@pts.se"
  - 0 issue "godaddy.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: pts.se
  spf: true
hosts:
- cert_expires: Mar 21 12:37:14 2027 GMT
  host: pts.se
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Pts Se Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Post- och telestyrelsen, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Post- och telestyrelsen
provider_slug: pts-se
slug: pts-se-domain-security
source_filename: pts-se-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pts.se\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 21 12:37:14 2027 GMT\n  hsts: false\ndomains:\n- domain: pts.se\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:postmaster@pts.se\"\n  - 0 issue \"godaddy.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pts-se/refs/heads/main/security/pts-se-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Government
- Telecommunications
- Postal Services
- Sweden
- Regulations
- Company
---
