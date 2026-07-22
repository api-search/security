---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: helloalice.com
  spf: true
hosts:
- cert_expires: Oct  5 19:21:29 2026 GMT
  host: helloalice.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hello Alice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hello Alice, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Hello Alice
provider_slug: hello-alice
slug: hello-alice-domain-security
source_filename: hello-alice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: helloalice.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:21:29 2026 GMT\n  hsts: null\ndomains:\n- domain: helloalice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hello-alice/refs/heads/main/security/hello-alice-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Fintech
- Small Business
- Grants
- Funding
- Entrepreneurship
- Lending
---
