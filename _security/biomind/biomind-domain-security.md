---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: biomindhealth.com
  spf: true
hosts:
- cert_expires: Nov 12 03:09:31 2026 GMT
  host: www.biomindhealth.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Biomind Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BioMind, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BioMind
provider_slug: biomind
slug: biomind-domain-security
source_filename: biomind-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.biomindhealth.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 03:09:31 2026 GMT\n  hsts: false\ndomains:\n- domain: biomindhealth.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/biomind/refs/heads/main/security/biomind-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Health
- Biotechnology
- Education
- Platform
---
