---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ntfy.sh
  spf: false
hosts:
- cert_expires: Jan 23 00:59:19 2027 GMT
  host: ntfy.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ntfy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ntfy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ntfy
provider_slug: ntfy
slug: ntfy-domain-security
source_filename: ntfy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ntfy.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 00:59:19 2027 GMT\n  hsts: false\ndomains:\n- domain: ntfy.sh\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ntfy/security/ntfy-domain-security.yml
summary_line: TLSv1.3
tags:
- Notifications
- Open Source
- Self‑hostable
- Pub‑Sub
- API
---
