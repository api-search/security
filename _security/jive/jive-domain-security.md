---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jivesoftware.com
  spf: true
hosts:
- cert_expires: Sep 29 16:31:55 2026 GMT
  host: www.jivesoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Jive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jive, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Jive
provider_slug: jive
slug: jive-domain-security
source_filename: jive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jivesoftware.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 29 16:31:55 2026 GMT\n  hsts: false\ndomains:\n- domain: jivesoftware.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jive/refs/heads/main/security/jive-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Enterprise
- Collaboration
- Digital Workplace
- Knowledge Management
- Intranet
- Enterprise Social
- Communication
---
