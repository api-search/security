---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: plainid.com
  spf: true
hosts:
- cert_expires: Sep  6 14:35:56 2026 GMT
  host: www.plainid.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Plainid Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for PlainID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: PlainID
provider_slug: plainid
slug: plainid-domain-security
source_filename: plainid-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.plainid.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 14:35:56 2026 GMT\n  hsts: false\ndomains:\n- domain: plainid.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plainid/refs/heads/main/security/plainid-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Cybersecurity
- Authorization
- Access Control
- PBAC
- Identity
- Policy Management
- API Security
---
