---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: braunintertec.com
  spf: true
hosts:
- cert_expires: Dec 17 02:31:55 2026 GMT
  host: www.braunintertec.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Brauninterteccorporation2 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Brauninterteccorporation2, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Brauninterteccorporation2
provider_slug: brauninterteccorporation2
slug: brauninterteccorporation2-domain-security
source_filename: brauninterteccorporation2-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.braunintertec.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 02:31:55 2026 GMT\n  hsts: false\ndomains:\n- domain: braunintertec.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brauninterteccorporation2/refs/heads/main/security/brauninterteccorporation2-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
---
