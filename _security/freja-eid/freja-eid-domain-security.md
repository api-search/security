---
description: ''
domains:
- caa:
  - 0 iodef "mailto:tac@frejaeid.se"
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: frejaeid.com
  spf: true
hosts:
- cert_expires: Mar 22 23:59:59 2027 GMT
  host: frejaeid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Freja Eid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Freja eID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Freja eID
provider_slug: freja-eid
slug: freja-eid-domain-security
source_filename: freja-eid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: frejaeid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 22 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: frejaeid.com\n  dnssec: true\n  caa:\n  - 0 iodef \"mailto:tac@frejaeid.se\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/freja-eid/refs/heads/main/security/freja-eid-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Identity
- Authentication
- DigitalSignature
- EU
- EEA
---
