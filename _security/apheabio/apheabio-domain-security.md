---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: aphea.bio
  spf: true
hosts:
- cert_expires: Oct 30 20:40:14 2026 GMT
  host: www.aphea.bio
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apheabio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Apheabio, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Apheabio
provider_slug: apheabio
slug: apheabio-domain-security
source_filename: apheabio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aphea.bio\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 20:40:14 2026 GMT\n  hsts: false\ndomains:\n- domain: aphea.bio\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apheabio/refs/heads/main/security/apheabio-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Agriculture
- Biotech
- Sustainability
- Biostimulants
---
