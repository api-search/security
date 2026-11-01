---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: devreply.com
  spf: true
hosts:
- cert_expires: Dec 27 11:52:11 2026 GMT
  host: devreply.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Devreply Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for devreply-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: devreply-com
provider_slug: devreply-com
slug: devreply-com-domain-security
source_filename: devreply-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: devreply.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 27 11:52:11 2026 GMT\n  hsts: false\ndomains:\n- domain: devreply.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/devreply-com/security/devreply-com-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Chat
- Customer Support
- Mobile
- Web
- Developer Tools
---
