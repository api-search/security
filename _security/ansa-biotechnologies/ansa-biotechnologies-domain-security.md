---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ansabio.com
  spf: true
hosts:
- cert_expires: Oct 19 11:38:23 2026 GMT
  host: ansabio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ansa Biotechnologies Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ansa Biotechnologies, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ansa Biotechnologies
provider_slug: ansa-biotechnologies
slug: ansa-biotechnologies-domain-security
source_filename: ansa-biotechnologies-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ansabio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 11:38:23 2026 GMT\n  hsts: false\ndomains:\n- domain: ansabio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ansa-biotechnologies/refs/heads/main/security/ansa-biotechnologies-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Biotechnology
- Synthetic Biology
- DNA Synthesis
- Gene Synthesis
- Life Sciences
- Laboratory Services
---
