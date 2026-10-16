---
description: ''
domains:
- caa:
  - 0 issuewild "harica.gr"
  - 0 issue "harica.gr"
  - 0 iodef "mailto:aai-is@lists.geant.org"
  - 0 issuewild "letsencrypt.org"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: geant.org
  spf: true
hosts:
- cert_expires: Nov 26 11:50:19 2026 GMT
  host: geant.org
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GEANT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GEANT
provider_slug: geant
slug: geant-domain-security
source_filename: geant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geant.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 26 11:50:19 2026 GMT\n  hsts: null\ndomains:\n- domain: geant.org\n  dnssec: false\n  caa:\n  - 0 issuewild \"harica.gr\"\n  - 0 issue \"harica.gr\"\n  - 0 iodef \"mailto:aai-is@lists.geant.org\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geant/refs/heads/main/security/geant-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
