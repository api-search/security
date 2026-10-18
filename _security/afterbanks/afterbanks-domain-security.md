---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: afterbanks.com
  spf: true
hosts:
- cert_expires: Dec 19 23:59:59 2026 GMT
  host: afterbanks.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Afterbanks Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Morpheus Aiolos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Morpheus Aiolos
provider_slug: afterbanks
slug: afterbanks-domain-security
source_filename: afterbanks-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: afterbanks.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 19 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: afterbanks.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/afterbanks/refs/heads/main/security/afterbanks-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- Fintech
- Artificial Intelligence
- Banking
---
