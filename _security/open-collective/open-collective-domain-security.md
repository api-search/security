---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: opencollective.com
  spf: true
hosts:
- cert_expires: Aug 31 02:36:11 2026 GMT
  host: docs.opencollective.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Open Collective Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Open Collective, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Open Collective
provider_slug: open-collective
slug: open-collective-domain-security
source_filename: open-collective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.opencollective.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 02:36:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opencollective.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-collective/refs/heads/main/security/open-collective-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Social
- Public APIs
---
