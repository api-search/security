---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: assiduusglobal.com
  spf: true
hosts:
- cert_expires: Dec 13 18:44:07 2026 GMT
  host: www.assiduusglobal.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Assiduusglobal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Assiduusglobal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Assiduusglobal
provider_slug: assiduusglobal
slug: assiduusglobal-domain-security
source_filename: assiduusglobal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.assiduusglobal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 18:44:07 2026 GMT\n  hsts: false\ndomains:\n- domain: assiduusglobal.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/assiduusglobal/refs/heads/main/security/assiduusglobal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- E-Commerce
- Artificial Intelligence
- Supply Chain
- Marketplace
- Brand Protection
- GlobalExpansion
---
