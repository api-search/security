---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ukrdigital.org
  spf: true
hosts:
- cert_expires: Dec  8 07:46:31 2026 GMT
  host: ukrdigital.org
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ukrdigital Org Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ukrdigital-org, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ukrdigital-org
provider_slug: ukrdigital-org
slug: ukrdigital-org-domain-security
source_filename: ukrdigital-org-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ukrdigital.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 07:46:31 2026 GMT\n  hsts: false\ndomains:\n- domain: ukrdigital.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ukrdigital-org/security/ukrdigital-org-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Charity
- Blockchain
- HumanitarianAid
- Ukraine
- Web3
- Nonprofit
---
