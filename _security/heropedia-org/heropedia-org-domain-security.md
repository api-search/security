---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: heropedia.org
  spf: true
hosts:
- cert_expires: Jan  8 08:18:45 2027 GMT
  host: heropedia.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Heropedia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heropedia, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Heropedia
provider_slug: heropedia-org
slug: heropedia-org-domain-security
source_filename: heropedia-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: heropedia.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 08:18:45 2027 GMT\n  hsts: false\ndomains:\n- domain: heropedia.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/heropedia-org/security/heropedia-org-domain-security.yml
summary_line: TLSv1.3
tags:
- Artificial Intelligence
- Mentorship
- Productivity
- LLM
- Office Hours
---
