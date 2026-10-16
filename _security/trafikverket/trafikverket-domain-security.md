---
description: ''
domains:
- caa:
  - 0 issuewild "telia.com"
  - 0 issue "telia.se"
  - 0 issue "telia.com"
  - 0 issuewild "telia.se"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: trafikverket.se
  spf: true
hosts:
- cert_expires: Feb  2 08:53:40 2027 GMT
  host: trafikverket.se
  hsts: true
  hsts_max_age: 157680000
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Trafikverket Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Trafikverket, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Trafikverket
provider_slug: trafikverket
slug: trafikverket-domain-security
source_filename: trafikverket-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: trafikverket.se\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  2 08:53:40 2027 GMT\n  hsts: true\n  hsts_max_age: 157680000\ndomains:\n- domain: trafikverket.se\n  dnssec: true\n  caa:\n  - 0 issuewild \"telia.com\"\n  - 0 issue \"telia.se\"\n  - 0 issue \"telia.com\"\n  - 0 issuewild \"telia.se\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trafikverket/refs/heads/main/security/trafikverket-domain-security.yml
summary_line: TLSv1.2 · HSTS · DNSSEC · DMARC
tags:
- Company
- Transport
- Government
- Sweden
- Infrastructure
---
