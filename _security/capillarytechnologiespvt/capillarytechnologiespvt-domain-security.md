---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: capillarytech.com
  spf: true
hosts:
- cert_expires: Nov 10 17:57:31 2026 GMT
  host: www.capillarytech.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capillarytechnologiespvt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capillarytechnologiespvt, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capillarytechnologiespvt
provider_slug: capillarytechnologiespvt
slug: capillarytechnologiespvt-domain-security
source_filename: capillarytechnologiespvt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.capillarytech.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 17:57:31 2026 GMT\n  hsts: null\ndomains:\n- domain: capillarytech.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capillarytechnologiespvt/refs/heads/main/security/capillarytechnologiespvt-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
---
