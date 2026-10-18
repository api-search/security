---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: connect2id.com
  spf: true
hosts:
- cert_expires: Dec 23 03:55:26 2026 GMT
  host: connect2id.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Connect2Id Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Connect2id, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Connect2id
provider_slug: connect2id
slug: connect2id-domain-security
source_filename: connect2id-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: connect2id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 03:55:26 2026 GMT\n  hsts: false\ndomains:\n- domain: connect2id.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/connect2id/refs/heads/main/security/connect2id-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- OpenID Connect
- Authentication
- Identity
---
